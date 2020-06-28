# AD-Password-Expiry-Notify

#
# Thanks meoso/Password-Expiration-Notifications.ps1

# Requirement :
# 1. AD password expiry notification email send using AWS SES SMTP 
# 2. It should be scheduled every day 10am. 
# 3. Encrypt the SMTP password
# 4. As my AD username is not an email ID, So I have updated the right email ID in the properties of the AD user respectively. 
# 14 days prior notification
# Use 587 port with SSL 

#  How to encrypt : Encrypt at the right path and mention that path in the $File variable 
# "AWS-SES-SMTP-PASSWORD" | ConvertTo-SecureString -AsPlainText -Force | ConvertFrom-SecureString | Out-File "C:\Users\Admin\Desktop\email\EmailPassword.txt"

