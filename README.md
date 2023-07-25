# Web_Recon
This is a Web Application Reconnaissance Tool
This appears to be a Python script for conducting subdomain enumeration, virtual host fuzzing, URL enumeration, directory brute-forcing, and parameter fuzzing. The script uses various command-line tools like `subfinder`, `assetfinder`, `httpx`, `ffuf`, `waybackurls`, and `gau` to perform the different tasks.

Here's a breakdown of what the script does:

1. It starts by defining some color codes for displaying banners and messages in different colors on the console, depending on whether the script is running on Windows or not.

2. The `banner()` function prints a banner with the name of the script's creator, presumably the person who coded it, and some ASCII art.

3. The user is prompted to enter the location where they want to store the gathered information and the domain they want to gather information about.

4. A folder is created at the specified location to store the results related to the given domain.

5. Subdomain enumeration is performed using `subfinder` and `assetfinder`, and the results are stored in a file called `live_subs.txt`.

6. Virtual host fuzzing is performed on the live subdomains using `ffuf`, and the results are stored in a file called `vhost.txt`.

7. URL enumeration is conducted using `waybackurls` and `gau` on the live subdomains, and the results are stored in a file called `urls1.txt`.

8. Directory brute-forcing is carried out using `ffuf` on the live subdomains, and the results are stored in a file called `directory_fuzzed.txt`.

9. Parameter fuzzing is performed using `ffuf` on the live subdomains, and the results are stored in a file called `parameters_fuzzed.txt`.

10. The script ends by printing a "Thanks for Using" message.

Please note that this script heavily relies on external tools like `subfinder`, `assetfinder`, `httpx`, `ffuf`, `waybackurls`, and `gau`, so these tools need to be installed and available in the system's PATH for the script to work correctly. Additionally, the script assumes the presence of two wordlists, `wordlist.txt` and `parameters.txt`, which are used for virtual host and parameter fuzzing, respectively. These wordlists need to be provided or edited in the script before running it.

Overall, this script seems to be a useful tool for conducting reconnaissance and information gathering during the initial phases of a security assessment or bug bounty hunting.
