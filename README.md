# Github-Configuration

# Install GIT Software
    https://git-scm.com/downloads
  
# Generating a new SSH key

   1) Open Terminal.
   2) Paste the text below, substituting in your GitHub Enterprise email address.
      ```
      ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
      ```
      
   3) When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.
       Enter a file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter]
       Enter passphrase (empty for no passphrase): [Press enter]
       Enter same passphrase again: [Press enter]

    4) Run the Agent
     
       eval "$(ssh-agent -s)"
    
       
    5) Adding your SSH key to the 

       ssh-agent ssh-add -K ~/.ssh/id_rsa
  
       
  # Adding a new SSH key to your GitHub account
  
     1) Copy the contents of the id_rsa.pub file to your clipboard 
        
     
        pbcopy < ~/.ssh/id_rsa.pub
   
        
     2) Login to https://git.soma.salesforce.com
        
     3) In the upper-right corner of any page, click your profile photo, then click Settings.
     
     4) In the user settings sidebar, click SSH and GPG keys.
     
     5) Click New SSH key or Add SSH key.
     
     6) In the "Title" field, add a descriptive label for the new key. For example, if you're using a          personal Mac, you might call this key "Personal MacBook Air".
     
     7) Paste your key into the "Key" field.
     
     8) Click Add SSH key.
     
     9) If prompted, confirm your GitHub Enterprise password.
