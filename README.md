# AUTOMATE RECON
A collection of bash scripts I wrote to automate my recon, as I am learning different recon methods. I will keep updating it and adding more stuff. This is just the stuff I am doing repeatedly, so y not put it in a bash script and save trouble for next time. 

### Recon.sh
After viewing @namasec first livestream, just followed and did stuff manually, and after that automate it, cause 
AUTOMATE EVERYTHING!!!!!!
The idea here is, to automate the process from finding subdomains, then unique subdomains and taking screenshots too.
And then sending the unique subdomains, again to script to do the same thing. 
I will add more stuff as I find time like port scanning and stuff.
If you have any bright ideas or want to automate something, just ping me at @codesceptre, 

##### Tools Required:
1. Subfinder
3. Httprobe
2. GoWitness

##### Usage:
./recon.sh $1 $2 $2
domain=$1 threads=$2 trimlvl=$3
Example: ./recon.sh example.com 10 4

### Alive.sh
Does same stuff, as recon but does not take screenshots.
Big idea here is, to find new targets or subdomains daily from a program and match it with existing alive.txt, new code everyday pushed by the company, keep an eye and AUTOMATE EVERYTHING!!!!!!
Command to check for new subdomains
sort oldReconSubdomains.txt newReconSubdomains.txt | uniq -u 
Gives domains that are not listed in oldReconSubdomains,txt, resulting in maybe new targets.
