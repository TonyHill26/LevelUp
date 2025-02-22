# Installing Hugo 0.120.3 on macOS (Apple Silicon)

Unfortunately this site won't run on recent versions of Hugo. And there's no option to simply tap an older version in Homebrew.

This guide documents the process of manually installing Hugo 0.120.3 on a Mac with an M1/M2/M3 processor and ensuring Homebrew does not update it.

## 0. Install the latest version using Homebrew

Run Homebrew: `brew install hugo`

## 1. Clone the Hugo Repository
Create a temporary directory and clone the Hugo source code for version `0.120.3`:
```sh
mkdir -p ~/tmp/hugo-aargh
cd ~/tmp/hugo-aargh
git clone --branch v0.120.3 --depth 1 https://github.com/gohugoio/hugo.git
cd hugo
```

## 2. Set Build Metadata
Retrieve the commit hash and current build date:
```sh
COMMIT_HASH=$(git rev-parse HEAD)
BUILD_DATE=$(date -u +"%Y-%m-%dT%H:%M:%SZ")
```

## 3. Compile Hugo with Extended Features
Build Hugo with the necessary flags:
```sh
go build -tags extended -ldflags "-s -w \
  -X github.com/gohugoio/hugo/common/hugo.commitHash=${COMMIT_HASH} \
  -X github.com/gohugoio/hugo/common/hugo.buildDate=${BUILD_DATE} \
  -X github.com/gohugoio/hugo/common/hugo.vendorInfo=brew" \
  -o hugo
```

## 4. Install the Compiled Binary
Move the compiled binary to `/opt/homebrew/bin/` and make it executable:
```sh
sudo mv hugo /opt/homebrew/bin/hugo
chmod +x /opt/homebrew/bin/hugo
```

## 5. Verify the Installation
Check that Hugo is installed and running the correct version:
```sh
hugo version
```

## 6. Prevent Homebrew from Updating Hugo
To ensure that Homebrew does not automatically update Hugo, pin the package:
```sh
brew pin hugo
```

You can confirm that `hugo` is pinned by running:
```sh
brew list --pinned
```

---

### **Notes**
- This method manually compiles Hugo instead of using `brew install` to avoid unwanted automatic updates.
- If a future update is needed, you can unpin it with:
  ```sh
  brew unpin hugo
  ```
- To remove the temporary build directory:
  ```sh
  rm -rf ~/tmp/hugo-aargh
  ```

Hugo 0.120.3 is now installed and locked from Homebrew updates! 🚀
