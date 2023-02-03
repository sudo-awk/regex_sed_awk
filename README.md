# regex_sed_awk
My scripts to manipulate bash script standard input and output stream

# THIS IS MY REGEX COMMANDS CREATED 

# FOR NMAP (To remove the first 4 lines and 4 last lines)
cat nmap_inital.txt | awk '{print $1}' | head -n -3 | sed 's#/tcp# # ' | tail -n +7

# to remove all whitespaces in stdout
tr -d ' \t\n\r'

# to replace new lines, into a comma
sed -z 's/\n/,/g;s/,$/\n/' 
