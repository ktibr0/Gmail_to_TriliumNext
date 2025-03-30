# Gmail_to_TriliumNext
Simple workflow to put your emails from gmail to Trilium


Download json file. edit line 56:
        **"url": "https://YOUR_N8N_Instance/etapi/create-note"**         
with your address of n8n instance. save file. 

You can do this later, when editing workflow at n8n interface.

        
Create worflow. Choose Import from file

![image](https://github.com/user-attachments/assets/e9532c35-9358-4956-8392-3d39d5e0cf38)

Upload json file.

Dbl click on http_request block and edit URL (if you haven't do it earlier) with your n8n address.

On Header_Auth inputbox choose :Create new credential" fill as shown at picture. Value must be Etapi token from TrilliumNext

![image](https://github.com/user-attachments/assets/2932f247-51c4-4525-ab09-330be6214f1f)



On TriliumNext interface add note (i call mine - Gmail), then click on it and in address line in browser copy ID of this node, between  green lines:
![image](https://github.com/user-attachments/assets/7219595f-5d79-4688-b39e-efe3debc8e25)

Fill this value to last parameter
![image](https://github.com/user-attachments/assets/037438fc-2647-4064-84e0-2f724fc0bc51)

or you can write Root, and all notes will be at first level of ierarchi

if you want, you may change Poll time at GmailTrigger, add some filters etc..
