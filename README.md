# gpt2AI_whatsapp_simulation
Fine tune Open AI's GPT2 on Whatsapp Chats to generate conversations
The following steps are for running a Colab notebook, you can also run it locally. In that case it'd take longer since you don't get Colab's GPUs and you'd also have to replace the google drive folders with local ones.

There are 4 versions of the pretrained model. I have used the second largest one (774M, Large, ¬3GB). Colab (free version) was frequently crashing with he extra-large model.
I won't be describing GPT-2 in detail, instead I'd encourage you yo check these if you are not familiar with it.

## Instructions
1. Export chats from Whatsapp mobile application

<img src="https://github.com/swahareddy/gpt2AI_whatsapp_simulation/blob/master/readme_images/WhatsApp%20Image%202020-08-02%20at%2011.52.43.jpeg" height="240" width="330"> <img src="https://github.com/swahareddy/gpt2AI_whatsapp_simulation/blob/master/readme_images/WhatsApp%20Image%202020-08-02%20at%2011.52.43%20(1).jpeg" height="240" width="340">

2. Create the following hierarchy in your google drive 
<img src="https://github.com/swahareddy/gpt2AI_whatsapp_simulation/blob/master/readme_images/gdrive_structure.png" height="240" width="330">

3. Upload the original_chat.txt in your google drive in the folder `Original Chats`

4. Run the jupter notebook on Google colab.

5. Check your output in the `Predicted Chats` folder

## Misc

* The training checkpoints can be backed up into `Chat models` in case you want to come back and use the fine-tuned model later. This code cell is commented by default since the checkpoint size is >3GB.

* The copy of files (`generated_text`) from Colab local runtime -> GDrive is a little slow, give it a couple of minutes

* Drop a mail at swahareddy@gmail.com for any comments.
