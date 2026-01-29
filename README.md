# Created an EC2 instance with the specifications as 20 GB storage and t3.micro and security group that allows inbound traffic on ports 22 (SSH), 80 (HTTP), 3000, 3001 (for web applications), and 27017 (MongoDB).  
  
<img width="1072" height="371" alt="image" src="https://github.com/user-attachments/assets/aa950082-bf38-4ce1-8d97-f367b46c2025" />    
<img width="886" height="155" alt="image" src="https://github.com/user-attachments/assets/f39355c2-ead5-49fc-a33d-872120576412" />    
  
### Update the VM, install docker and docker compose using below commands.  
sudo apt update  
sudo apt install -y docker.io docker-compose  
  
### Added user ubuntu to the group docker  
sudo usermod -aG docker ubuntu  
  
### Clone the Travel Memory git repository into the VM.  
git clone https://github.com/UnpredictablePrashant/TravelMemory.git  
  
### Create dockerfiles for both backend and frontend  
<img width="382" height="108" alt="image" src="https://github.com/user-attachments/assets/dcae2e51-3df7-4940-8c9c-f212d0cefa7b" />  
  
<img width="374" height="110" alt="image" src="https://github.com/user-attachments/assets/1d553758-bb62-4df8-be83-aaa2afbf859d" />  
  
### Build Images using the below commands  
docker build -t backend .  
docker build -t frontend .  
  
<img width="422" height="49" alt="image" src="https://github.com/user-attachments/assets/385b656b-c767-4d48-8d1b-3abf5f5d99e7" />  



