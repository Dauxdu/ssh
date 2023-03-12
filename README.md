Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0

ssh-keygen -t ed25519

Set-service ssh-agent StartupType ‘Automatic’
Start-Service ssh-agent

ssh-add "C:\Users\User\.ssh\id_ed25519"
