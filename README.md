# one-liner nuclei 
cat subdomains.txt | while read subdomain; do nuclei -t /path/to/templates/ -u $subdomain -o nuclei_output.txt; done

# one-liner jaeles 
cat subdomains.txt | while read subdomain; do jaeles scan -s /path/to/signatures/ -u $subdomain -o jaeles_output.txt; done
