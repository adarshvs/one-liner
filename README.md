# one-liner nuclei 
cat subdomains.txt | while read subdomain; do nuclei -t /path/to/templates/ -u $subdomain -o nuclei_output.txt; done
