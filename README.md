# ln-scoring-algorithm-updated

A program to find the optimal outfit + top 20 scoring items for association, chapter, arena, and custom stages in Love Nikki. This program requires your clothes_date file to run. Please refer to any of the guides out there for extracting this file; Nikki's Info also accepts it for wardrobe information, so many guides exist. 

Your clothes_date file MUST be renamed to **clothes_date.txt** and it MUST be in the same folder as the executable.

Blacklisted items are not accounted for. Please refer to other community resources to identify and avoid blacklisted items. Similarly, chapter requirements are not considered.

If there is a newer version of the executable, that version likely has additional clothes or stages added. Please download that version if you want to access new clothes and new stages.

Please contact _________ on Discord for any bugs, questions, or concerns. 

# macOS

### Requirements: 

- macOS Tahoe 26.1 or above (You can try older versions, I can't guarantee it'll work.)
- Your clothes_date file


### Running the executable on first launch:

The steps below assume you are keeping the executable in your Downloads folder. It will work in other folders; however, the cd command will require a different file pathway.

1. Open Terminal.
2. Type in the following commands. 
      - cd Downloads
      - xattr -d com.apple.quarantine "LNScoringAlgo" 
      - chmod +x "LNScoringAlgo"
3. Open Finder.
4. Check that...
      - Your clothes_date file is in the Downloads folder.
      - Your clothes_date file has been renamed to clothes_date.txt
5. Run the executable! There are two ways to do so:
      - Double click on the LNScoringAlgo file
      - Type ./LNScoringAlgo into Terminal.
  
### Running the exectuable on later launches:

It is still assumed that you are keeping the executable in your Downloads folder.

#### Running Through Terminal

  1. Open Terminal
  2. Type in the following commands:
        - cd Downloads
        - ./LNScoringAlgo

#### Running through Finder

  1. Open Finder
  2. Open the Downloads folder
  3. Double click on the LNScoringAlgo file


As long as you don't move anything, you should be able to keep launching LNScoringAlgo without any issues. (If you want to launch it through You will have to go through steps 1 and 2 again every time you re-download the executable.

# Usage

So. How the hell do you use this thing? Well, it depends on the type of stage you want an outfit for!

### <ins> Arena <ins>

When the program prompts you to "Enter stage code:", type in A. 

The program will print out a number and the names of arena stages. Type in the number that corresponds with the arena stage when prompted.

###  <ins> Commission Stages <ins> 

When the program prompts you to "Enter stage code:", type in GA_S_.

Fill in the blank spaces with the act number and stage number for the stage you want to play. 

For example:

You want to play 1-1 Pajamas Party. You will type in GA1S1. 

You want to play 6-3 New manga inspiration. You will type in GA6S3.

You want to play 20-7 The Sound of Stars. You will type in GA20S7.

### <ins> Custom Stages <ins>

When the program prompts you to "Enter stage code:", type in C. 

Follow the prompts given. 

###  <ins> Maiden Stages <ins> 

When the program prmpts you to "Enter stage code:", type in MV_C_S_.

Fill in the blank spaces with the volume number, chapter number, and stage number for the stage you want to play. For side stages, add a S in front of the stage number.

For example:

You want to play V1:1-1 Sport Girl Aron (1). You will type in MV1C1S1.

You want to play V1:7-S2 Toto, Girl in Love (6). You will type in MV1C7SS1. 

You want to play V3:2-7 Reunion. You will type in MV3C2S7. 

###  <ins> Princess Stages <ins> 

When the program prmpts you to "Enter stage code:", type in PV_C_S_.

Fill in the blank spaces with the volume number, chapter number, and stage number for the stage you want to play. For side stages, add a S in front of the stage number.

For example:

You want to play V1:1-1 Sport Girl Aron (1). You will type in PV1C1S1.

You want to play V1:7-S2 Toto, Girl in Love (6). You will type in PV1C7SS1. 

You want to play V3:2-7 Reunion. You will type in PV3C2S7. 


# FAQs

**Why isn't this a website?**

Websites cost money to run. I don't want to pay that money. Also, I don't know how to code a functioning website.

**Is this a virus?**

No. I don't know how to code that either. However, you should never give any random file off the internet the permissions this needs in order to run on Mac -- *if* it was a virus, you'd be screwed. It needs these permissions because I can't sign the executable , and from what I gather, you need to purchase a membership to the Apple Developer Program in order to get a signing certificate. 

This file was written in Python, then turned into an executable for distribution and ease of use using PyInstaller. As far as I know, neither contain malware. 

**Why should I use this over Nikki's Info?**

It's more up-to-date. It has the latest association and chapter stages, as well as new clothes that Nikki's Info doesn't have yet. However, Nikki's Info is fine for the vast majority of people, it works on mobile, and it lets you input items manually. Nikki's Info is still an excellent option.

**Why do you and Nikki's info list different base scores/item scores?**

I don't know, but in my testing, the overall outfits were pretty much the same, so I'm not very concerned about the exact numbers.

**Item X scores a few points higher than Item Y! How much will it affect my scoring?**

It pretty much won't. 


**Can I delete those .txt files it keeps spitting out?**

Yes. They're only there to store what your optimal outfit + the top 20 scoring items for a stage are, so you can see them even after you close the program.

# Acknowledgements

crescendont - main contributor, maintainer

danc12321 - additional contributions, testing, maintainer

______ - testing

Many thanks to Nikki's Info for being a long-standing community resource, as well as a sanity check for our program.
