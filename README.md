![PXL_20250220_183435246](https://github.com/user-attachments/assets/b34cade0-82b3-4d29-89b0-fb2c501141b5)

# Introduction
I've been wanting to store some of my raw photos from astrophotography onto my computer, but I was getting worried about my overall storage. For this reason, I decided to embark on a project to create a NAS - network-attached storage - based on the Pi 5 system. This proved to be much harder than I initially thought it was going to be, but let's get to it. I followed this guide to help me out: https://www.the-diy-life.com/i-built-a-4-bay-raspberry-pi-5-based-nas/

# Material(s)

The following materials are used for this NAS.

Vemico Raspberry Pi 5 Kit 8GB RAM with 32GB Card Readers Kit, 27W 5.1V5A PD Power Supply for Raspberry Pi 5, Aluminum Heatsinks 4pcs and Raspberry Pi 5 8GB Board - this can be purchased for $105.99 at the following link: https://www.amazon.com/Raspberry-4GB-Board-Heatsinks-4pcs/dp/B0CQ2WGZFG/ref=sr_1_20?crid=IMS3RTKXPPQ7&dib=eyJ2IjoiMSJ9.W5N9lppf7Ww6euC0QW7Li84S4Lp1f8JEkyJjNIXAEypYcBvFPspduSUBebS0QrIVnvn2XiiPAWlgs5i7B9ZZw-quOd5WN4X0iBgyIo5laFzvKqvGheVNJZDJqBQ3mTooPS7GR-NR12PQBcO4qTQRJl0NyZSZn2IbnByfGnqoo5zV0iCz_HkMkBBA9AbRYisnQG10gUOBJ4BPTSHqV3qaxtae8IABCqpEQdhhkhS1-rc.aYtG4XG4nhzIcNAZjkTd20ZIzlUyrNxcPA-mC0crZ-w&dib_tag=se&keywords=raspberry%2Bpi%2B5%2B8gb&qid=1737497894&sprefix=raspberry%2Bpi%2B5%2Caps%2C160&sr=8-20

Vilros Raspberry Pi 5 Active Cooler with Compatible Holder, Quality Metal Heatsink & Variable-Speed Fan, Fully Vented for Maximum Airflow, Quiet & Software-Controlled (Board Not Included) - this can be purchased for $12.99 at the following link: https://www.amazon.com/Raspberry-Active-Vilros-Compatible-Acrylic/dp/B0CLM7KCVH?crid=3MCEIDG6G4K1L&dib=eyJ2IjoiMSJ9.8SjWj5QxttRkyl5s0KrfoxmD4ZMDk3GKbRWbBF12SxtaAaeonzeonph3XavcPRqD0xpp_00ytUyq-iq8a2z4_efE0Jl4VlcPnvHetqiWMnrxn7q3xJ9Q3JzpSqTICW5fioj9a2G5zI8d8YX1dYnm9T8leecpuJF8VpVK6ACDtB9yMPu0uVfOA0XpLTeUAUOeH0I-duvXy2Q4CyxmkAL-HbEoP-V7tdsAvsoFlYiwcxs.LHkVg-ERAG3aB0G-9lddQQrRADcB7EvfNEuEaGKLXB8&dib_tag=se&keywords=pi+5+active+cooler&qid=1715556822&sprefix=pi+5+active+cool,aps,267&sr=8-2-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1&linkCode=sl1&tag=mklements-20&linkId=79d9c8db37224dc80b5c97b1156c2fc8&language=en_US&ref_=as_li_ss_tl

Raspberry Pi 5 Penta SATA HAT - Up to 5X SATA Disks HAT - this can be purchased for $75.99 at the following link: https://www.amazon.com/Raspberry-Pi-Penta-SATA-HAT/dp/B0DCK4BHJK/ref=sr_1_1?dib=eyJ2IjoiMSJ9.PGNT7jfvq3uMK2Ll-Hd6fJ-L1ySMYafqL7ocNhF8hKKbuaZntph1hVQxO0dJ4XYVdd7dRIHy_Uu3ikUFbEzxWNeWmbAYOjdY_inro6v-HoR8Uvw5ZwXcyLkwMdi8PjL4SsY0rPrv4P_vbDRgazO15QoTLq6VJJeCV7IpECnqK1jie0wD9LnIIWKVac5CfqEfuuKtSeSb5wcX6d7loobLlLAIBfcdzbbxCMvZW1j7Y4U.tdArp6D-L95GuK6JwqNIcdJWHkgWThXdhgSFsvcw0pA&dib_tag=se&keywords=penta+sata+hat&qid=1736357005&sr=8-1

Crucial BX500 1TB 3D NAND SATA 2.5-Inch Internal SSD, up to 540MB/s - CT1000BX500SSD1, Solid State Drive - this can be purchased for $58.59 at the following link: https://www.amazon.com/Crucial-BX500-NAND-2-5-Inch-Internal/dp/B07YD579WM/ref=sr_1_3?crid=3SGVHSACN4BDU&dib=eyJ2IjoiMSJ9.Ye3VHf0Z0RC7v-rUDvfl2huASmBBKDUvucLkc6D9cTNbg-YhPmtybPI2nNl0Bg8rbi-qfKzi1i8YJ_q_uUlhfOcr9j7KOGBk6pPRbcqS2jlpEvKtA3Y9CpnwiHBGpY_4N-k3v_ImSGun1AUisn9HAXiCfH77rSURcao2vGu94ud5_2vCTQrW5b2AqQt5s4yYWL5t9M6mgfbjFo2qwSc6rhmR3ug0CANcFnlceByL8DY.8dYIwhZbAhoE6yABZrDH6tmMOFcGhd1H6k-tInrGKVs&dib_tag=se&keywords=2.5%22%2Bssd&qid=1736360605&sprefix=2.5%2Bssd%2Caps%2C94&sr=8-3&th=1

12V 3A AC Adapter Power Supply Charger [12 Volts 3 Amps Regulated Switching Power] with 11 Interchangeable DC Plug for 500mA 600mA 700mA 800mA 900mA 1000mA 1500mA 2000mA 2500mA 3000mA Equipment - this can be purchased for $14.99 at the following link: https://www.amazon.com/Adapter-Regulated-Switching-Interchangeable-Equipment/dp/B0BFPZ81B6?crid=32ALOG36NGP3P&dib=eyJ2IjoiMSJ9.Ev9obzVE7BHhlHQASM4eNe7--XA4ahA_OVUaUhmTI1gbqu59GYxwhAVR9d9qWN8fBHGSQdPBdzeWE5mp8CHt-PlMGNAtzV2AMFGNS9kRyztxqRd4WeUglt4zDSZGpc-8NN6zrlFWEDfjqlvV-B0A9JOknrWgo_aUvkmimv9u4WW8sEVuy3dMBNG4Idbiiji_CoL1R4tOpiYC4cQTcqGzHN5CsO4qrqvnRw1t2jBnlwY.8rqIiN6gOG8LqL7y19-_DsnVLC7ubIedKi-omXC9LRE&dib_tag=se&keywords=12v+3a+power+supply&qid=1715556783&sprefix=12v+3a+power+supp,aps,278&sr=8-2-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&psc=1&linkCode=sl1&tag=mklements-20&linkId=359116530adc81165887e3a376eb49b2&language=en_US&ref_=as_li_ss_tl
 
The Penta SATA HAT can fit 4 of the 2.5-inch SSDs, but I decided to just go with one for now because I want to test the system and make sure everything works before fully committing to 4. In any case, this project can cost somewhere between $268.55 and $444.32, which is cheaper than what most ready-made NAS cost.

# Assembly

The first step in assembling is attaching the active cooler to the Pi 5. Do so as shown below.

![PXL_20250219_141949804](https://github.com/user-attachments/assets/1dd3d87d-2778-4192-838a-bcb5e07a1cfc)

However, the SATA HAT needs some space, so use a pair of needle-nose plyers to remove the bottom left three pins on the active cooler. It should look like the image below.

![PXL_20250219_142701262](https://github.com/user-attachments/assets/d86cbaaf-e19e-4fba-b0fe-0fde5e558192)

Now, use the included offset stands to provide support for the SATA HAT. Make sure to plug in your active cooler in the top right part of the image below as well.

![PXL_20250219_143057575](https://github.com/user-attachments/assets/e439a2cc-6bc3-4a13-9b27-b1693b2f4d18)

Now, connect your SATA HAT's FPC cable as shown below.

![PXL_20250220_183057607](https://github.com/user-attachments/assets/d97b014d-c775-41c1-822c-11b6c12dc6b7)

Now, screw your SATA HAT on top like so:

![PXL_20250220_183330314](https://github.com/user-attachments/assets/33681d43-1261-4c2f-ad5e-04ade8bc85ee)

The last step is adding the SSD. Add as many as you bought (for me, it's just one for now). Below is what mine looks like.

![PXL_20250220_183354011](https://github.com/user-attachments/assets/a149d74b-c6f0-4f36-8120-ae8bde1354aa)

# Preparing the Software

Take the included microSD card and, using Pi Imager, upload Pi OS Lite. However, at the following screen, select "Edit Settings"

![image](https://github.com/user-attachments/assets/e223f0d8-d374-45e6-a49c-1bd9f5139a29)

Here, go to General and set a username and password as well as a hostname. Then, set Enable SSH under Services.

![image](https://github.com/user-attachments/assets/0374fe5b-52f8-427c-b18d-f47a166ffc3c)

Now, press save then "yes" for the following screens.


# First Boot

Once the OS is done, insert it into you Pi 5 and connect the Pi 5 to Ethernet and power it through the 12V power supply. Wait a few minutes for the Pi to boot up.

Use something like Angry IP Scanner (https://angryip.org/download/#linux) to find the IP address of the Pi5nas.

![image](https://github.com/user-attachments/assets/ac21522f-557e-4834-b93e-b33ae49dee5f)

Once you have done this, you can SSH into the Pi using the IP address. I decided to use termius on linux as my SSH tool. I copied my pi5nas's IP into the IP or Hostname then created a host.

![image](https://github.com/user-attachments/assets/1549309d-483c-4186-8e45-db3b3559597d)

I then logged in using the username and password I created previously for the pi5nas.

![image](https://github.com/user-attachments/assets/d41c717b-8c29-4322-a08b-a82600f06fd6)

From OpenMediaVault (https://github.com/OpenMediaVault-Plugin-Developers/installScript), I ran this line:

```bash
sudo wget -O - https://github.com/OpenMediaVault-Plugin-Developers/installScript/raw/master/install | sudo bash
```

![image](https://github.com/user-attachments/assets/35d97064-c0bc-4ed0-aa6d-d406d35acd8d)

It should take a few minutes to run. Then, it will reboot your pi and terminate the SSH session. You will likely see this:

![image](https://github.com/user-attachments/assets/98f30194-a1fc-45e9-9353-c577c3df27ef)

The IP has likely changed, so use Angry IP Scanner again to find it and then reconnect.

# Enabling PCIe Port on Pi

One of the last things we need to do is to enable the PCIe port on the pi. Run the following command:

```bash
sudo nano /boot/firmware/config.txt 
```

![image](https://github.com/user-attachments/assets/dca230d7-e6c9-4064-a86a-09026a451990)

And then add the following set of lines above [cm4]:

```bash
# Enable PCIe Port and Set to Gen 3 Speed
dtparam=pciex1
dtparam=pciex1_gen=3
```

![image](https://github.com/user-attachments/assets/a417d217-d6ec-4f4d-a32f-49b77a9217bd)

Press Ctrl+X, then Y, then Enter. Now, reboot the pi.

# Logging in and Connecting

We should now be able to access the Pi remotely by entering its IP address into our browser. Do another scan using the Angry IP Scanner and then copy the IP from it and paste it into your browser.

![image](https://github.com/user-attachments/assets/12f805e0-34f1-47e6-a635-dd25de121e51)

The default username is admin and default password is openmediavault. You should change your password after logging in. You should also update your system.

Then, go Storage -> Disks. Here, you should see your mounted disks.

![image](https://github.com/user-attachments/assets/44eb4b20-17e1-4135-96b4-e8bff13b1d52)

Now, go over to File Systems and select the create option. Select the BTRFS option and set the Profile as "Single" and select the SATA Disk then save.

![image](https://github.com/user-attachments/assets/a17248e5-cc2e-4c93-9158-216be5ea1ecc)

In the next screen, select the formatted volume and save again and then apply.

![image](https://github.com/user-attachments/assets/c4961dac-4d11-49f1-83ec-55a95494f8f9)

Now go to Shared Folders and select create. Name your folder, select the file system, and then click save.

![image](https://github.com/user-attachments/assets/64cae47c-7ab7-4e65-bbf0-d95d3cb5d4ea)

In the next screen, click apply.

# Crucial Services

To make sure that this NAS is viewable to Linux and MacOS machines, go over to Services then click on NFS followed by Settings. Select Enabled.

![image](https://github.com/user-attachments/assets/a941eeba-13e1-49fc-948d-4bd815012d6c)

Now, select save and then apply.

To make sure that this NAS is also viewable to Windows machines, click on SMB/CIFS, Settings, and then Enabled for Workgroup.

Hit save and apply in the subsequent screen.

![image](https://github.com/user-attachments/assets/28a07681-79ca-42ab-9336-268c853986f4)

We must now go over to Services then SMB/CIFS. Here, select Settings then Enabled for Workgroup. Hit save at the bottom and apply when available.

Go over to "Shares" and then create a new share. Here, select the folder just created earlier and click save right after and apply.

![image](https://github.com/user-attachments/assets/bfe781f5-935c-4584-8108-efa999df40ce)


Then, go to Services -> SMB/CIFS -> Settings and select Enabled for the Workgroup and below Home directories.

# Tips

I would recommend probably creating a better cooling solution, probably similar to the one from the guide I followed; however, I only wanted one SSD for right now.
