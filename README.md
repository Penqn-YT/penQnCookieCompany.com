Some reason the password dialog pop-up does NOT accept the login credentials when origin is mapped to GiHub.
May have cached the old password entries
Clear the origin by removing the oringin
And try

Code:
# List remote repositories (confirm origin exists)
git remote -v

# Remove remote origin
git remote remove origin

# Verify removal
git remote -v

git status      -- no entries in the output list

Enter the entries that were given when created a repository 
git remote add origin https://github.com/Yoururl/yourproject/yourname.com
git branch -M main
git push -u origin main

Popup: your token instead the password

Volah!
YT
