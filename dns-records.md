# DNS records

Just for reference!

| Domain Name | TTL | Record Type | Value |
|-------------|-----|-------------|-------|
| levellingupstem.co.uk | 3600 | NETLIFY | nifty-ptolemy-7d5b1d.netlify.app |
| www.levellingupstem.co.uk | 3600 | NETLIFY | nifty-ptolemy-7d5b1d.netlify.app |
| levellingupstem.co.uk | 3600 | NETLIFYv6 | nifty-ptolemy-7d5b1d.netlify.app |
| www.levellingupstem.co.uk | 3600 | NETLIFYv6 | nifty-ptolemy-7d5b1d.netlify.app |
| autodiscover.levellingupstem.co.uk | 3600 | CNAME | mail9.hostinguk.net |
| mail.levellingupstem.co.uk | 3600 | CNAME | mail9.hostinguk.net |
| smtp.levellingupstem.co.uk | 3600 | CNAME | mail9.hostinguk.net |
| levellingupstem.co.uk | 3600 | MX | 10 mail9.hostinguk.net |
| levellingupstem.co.uk | 3600 | MX | 50 mail.hostinguk.net |
| _dmarc.levellingupstem.co.uk | 3600 | TXT | v=DMARC1; p=quarantine; rua=mailto:devops.pr52@levellingupstem.co.uk; fo=1 |
| 8DBE9DA21AE6B99._domainKey.levellingupstem.co.uk | 3600 | TXT | p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA37QSn3ZxRSVElBawUis9rn2mTLTeFG44lbAefKf+PyIc8GL0ueEllpGB+8PT8aux7LhAU9m8ghqzcRWotXsldjiGPSUWqlaGvzh2QNkPJtXrfVyH9bIhJq52vM6tCXurc4jMwmdEy0alN/7HCWGQhxcCgPIPptBTInJP1CfVJfaW/W/LoEhHLexPIf+Y5xBoJSLHuRasmce/K0vP+r4tRrHsEz2c43Xpdee0KEWn6XAaelP1veufmpuE3Q4C7urqENSgDeEZtHWCrnO/LpnuJ5tFvnR0HvAbAAE6Ru/grNRkxmc9/xOTx9s/lLGPbGvFsn3HjJHxlbhoVPDez5QumQIDAQAB |
| levellingupstem.co.uk | 3600 | TXT | v=spf1 mx a include:smtpout.hostinguk.net -all |
| share.levellingupstem.co.uk | 3600 | CNAME | nextcloud.levelup.x.mythic-beasts.com. |

In raw format:
```txt
levellingupstem.co.uk	3600	NETLIFY	nifty-ptolemy-7d5b1d.netlify.app
www.levellingupstem.co.uk	3600	NETLIFY	nifty-ptolemy-7d5b1d.netlify.app
levellingupstem.co.uk	3600	NETLIFYv6	nifty-ptolemy-7d5b1d.netlify.app
www.levellingupstem.co.uk	3600	NETLIFYv6	nifty-ptolemy-7d5b1d.netlify.app
autodiscover.levellingupstem.co.uk	3600	CNAME	mail9.hostinguk.net
mail.levellingupstem.co.uk	3600	CNAME	mail9.hostinguk.net
smtp.levellingupstem.co.uk	3600	CNAME	mail9.hostinguk.net
levellingupstem.co.uk	3600	MX	10 mail9.hostinguk.net
levellingupstem.co.uk	3600	MX	50 mail.hostinguk.net
_dmarc.levellingupstem.co.uk	3600	TXT	v=DMARC1; p=quarantine; rua=mailto:devops.pr52@levellingupstem.co.uk; fo=1
8DBE9DA21AE6B99._domainKey.levellingupstem.co.uk	3600	TXT	p=MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEA37QSn3ZxRSVElBawUis9rn2mTLTeFG44lbAefKf+PyIc8GL0ueEllpGB+8PT8aux7LhAU9m8ghqzcRWotXsldjiGPSUWqlaGvzh2QNkPJtXrfVyH9bIhJq52vM6tCXurc4jMwmdEy0alN/7HCWGQhxcCgPIPptBTInJP1CfVJfaW/W/LoEhHLexPIf+Y5xBoJSLHuRasmce/K0vP+r4tRrHsEz2c43Xpdee0KEWn6XAaelP1veufmpuE3Q4C7urqENSgDeEZtHWCrnO/LpnuJ5tFvnR0HvAbAAE6Ru/grNRkxmc9/xOTx9s/lLGPbGvFsn3HjJHxlbhoVPDez5QumQIDAQAB
levellingupstem.co.uk	3600	TXT	v=spf1 mx a include:smtpout.hostinguk.net -all
share.levellingupstem.co.uk	3600	CNAME	nextcloud.levelup.x.mythic-beasts.com.
```
