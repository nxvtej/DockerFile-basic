optimize docker file to maintain max cache into image 

![image](https://github.com/user-attachments/assets/78bebc20-13e9-4621-ad76-d7f9b328a7c5)


![image](https://github.com/user-attachments/assets/e5c18591-824d-4761-a7e1-fb69ef908b0f)

add volume database


  data/db is deafult location for mongodb will be different for postgress 
    docker run -d -v volume_data:/data/db/ -p 27017:27017 mongo


add network to connect containers with another conatainers

![image](https://github.com/user-attachments/assets/7727752a-b187-4798-b3b8-60e72c653fa8)
from week 15 live 2.2
