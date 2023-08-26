## Rayder Workflows

 Repo for hosting rayder workflows. Install [Rayder](https://github.com/devanshbatham/rayder/) from [here](https://github.com/devanshbatham/rayder/)



## Workflows




| Category | Workflow                            | Description                                                | Placeholder(s)             | Dependencies                                                      |
|----------|-------------------------------------|------------------------------------------------------------|----------------------------|-------------------------------------------------------------------|
| Recon    | [generate-dns-wordlist.yaml](https://github.com/devanshbatham/rayder-workflows/blob/main/recon/generate-dns-wordlist.yaml) | Generate custom DNS Bruteforce wordlist for a domain | {{DOMAIN}}, {{OUTPUT_DIR}}  | [subfinder](https://github.com/projectdiscovery/subfinder), [dnsgen](https://github.com/ProjectAnte/dnsgen) |
| Scanning | [open-redirect.yaml](https://github.com/devanshbatham/rayder-workflows/blob/main/http/open-redirect.yaml) | Scan for Open Redirect vulnerabilities in params found in web archive for a domain | {{DOMAIN}}, {{OUTPUT_DIR}} | [Paramspider](https://github.com/devanshbatham/Paramspider), [Openredirex](https://github.com/devanshbatham/Openredirex) |
| Scanning | [xss-wayback.yaml](https://github.com/devanshbatham/rayder-workflows/blob/main/http/xss-wayback.yaml) | Discover potential XSS vulnerabilities on the URLs stored in Wayback archive for a domain | {{DOMAIN}}, {{OUTPUT_DIR}} | [waybackurls](https://github.com/tomnomnom/waybackurls), [qsreplace](https://github.com/tomnomnom/qsreplace), [httpx](https://github.com/projectdiscovery/httpx) |
| Recon    | [check-alive-ips.yaml](https://github.com/devanshbatham/rayder-workflows/blob/main/recon/check-alive-ips.yaml) | Check alive IPs (port 80, 443) for a file containing target IP addresses or ranges | {{TARGETS_FILE}}, {{OUTPUT_DIR}}, {{RATE}} | [masscan](https://github.com/robertdavidgraham/masscan) |
| Scanning | [header-brute.yaml](https://github.com/devanshbatham/rayder-workflows/blob/main/http/header-brute.yaml) | Brute force HTTP headers on a list of URLs | {{URLS_FILE}}, {{HEADERS_FILE}}, {{OUTPUT_DIR}} | [headerpwn](https://github.com/DevanshBatham/HeaderPwn) |
| Recon | [mutate-subdomains-radamsa.yaml](https://github.com/devanshbatham/rayder-workflows/blob/main/recon/mutate-subdomains-radamsa.yaml) | Mutate subdomains of a domain using radamsa and resolve using massdns | {{DOMAIN}}, {{OUTPUT_DIR}} | [massdns](https://github.com/blechschmidt/massdns), [radamsa](https://gitlab.com/akihe/radamsa), [getresolvers](https://github.com/devanshbatham/getresolvers), [subfinder](https://github.com/projectdiscovery/subfinder) |
| Scanning | [crlf-scan.yaml](https://github.com/devanshbatham/rayder-workflows/blob/main/http/crlf-scan.yaml) | Scan for CRLF vulnerabilities in subdomains of a domain | {{DOMAIN}}, {{OUTPUT_DIR}} | [subfinder](https://github.com/projectdiscovery/subfinder), [httpx](https://github.com/projectdiscovery/httpx), [crlfuzz](https://github.com/dwisiswant0/crlfuzz) |