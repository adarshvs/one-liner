# one-liner nuclei 
cat subdomains.txt | while read subdomain; do nuclei -t /path/to/templates/ -u $subdomain -o nuclei_output.txt; done

# one-liner jaeles 
cat subdomains.txt | while read subdomain; do jaeles scan -s /path/to/signatures/ -u $subdomain -o jaeles_output.txt; done

# one-liner dirsearch 
sudo dirsearch -l /home/domains.txt  -e* -f -o dirsearch-out.txt


# one-liner nikto 
nikto -h urls.txt -o results.txt
