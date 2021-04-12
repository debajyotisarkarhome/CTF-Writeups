# Problem : Parcel

'' That's a lot of magick ''

## Analysis

So this one was time consuming (Or maybe I'm a idiot who did it manually). So the [file](https://drive.google.com/file/d/1kUHoGNVqKaB3OHJdkbQ7X__HaV7pK30T/view?usp=sharing "file") supplied with it was a zip file which can be opened with 7zip or any archive manager. It had a text file with inside it with a lot of base64 encoded Email data, by seeing the MIME info I filtered the PNG/Image ones and used [cyberchef](https://0x1.gitlab.io/code/CyberChef/ "cyberchef") to convert each of the data sides into an image and used photoshop to puzzle them into a whole .
It looked something like this :
![Parcel)](https://raw.githubusercontent.com/lasq88/CTF/main/ritsec2021/forensics/parcel/puzzle2.PNG)

P.S. I forgot to save mine so I'm using the picture from [here](https://raw.githubusercontent.com/lasq88/CTF/main/ritsec2021 "here")