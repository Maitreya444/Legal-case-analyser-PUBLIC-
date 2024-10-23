# Legal-case-analyser-PUBLIC-
This is just readme. The actual project is private as it was a freelance project.

# Legal-Case-Analyser

Objectives:
1. Monitor Sources: Automatically track relevant sources for new case law decisions on legal costs.
2. Document Management: Save identified court judgments to OneDrive for easy access and sharing.
3. Summarisation: Read and summarise court judgments, highlighting key points and outcomes.
4. Notification: Circulate the summarised information to the team via email.

Freelance Project 1: 

Developed a robust web scraper capable of efficiently extracting over 100 legal documents daily from the UK High Court website and 5 other legal sources, significantly streamlining data collection and analysis for legal professionals.
Designed advanced Python scripts to summarize legal documents, reducing manual research time by 90% for solicitors.
Automated the delivery of 100 legal case summaries per day via email to 50 solicitors, seamlessly integrating with Google Drive to streamline document storage and access thus resulting in a 75% reduction in manual data handling and 20 hours saved per week for legal professionals.
 
1. Web Scrapers :
   Scraped Baili [Baili.org,](https://www.bailii.org/recent-decisions.html) 
   Scraped CivilLitigationBrief https://www.civillitigationbrief.com/
   Scraped CostBarrister https://costsbarrister.co.uk/
   Scraped https://www.lawgazette.co.uk/
   Scraped Posts from Sean Linley on LinkedIn

   For scraping Baili libraries like beautifulsoup were used.
   For scraping Linkedin post selenium web driver was used.
   For scraping the rest of the articles RSS feeds were used. Article and feedparser modules were used from python.

   We scraped them and saved into the local storage of the device in text format to apply further NLP.

2. Summarisers :
   Since the legal sources are scraped we need to summarize them according to this template.
   
   Name of Case: 
   Court in which heard: 
   Determining Judge: 
   Issue to be considered: 
   Question for the Court:
   Claimant's Position: 
   Defendant's Position: 
   Issues considered by the Judge:
   Case Law referenced in decision: 
   Outcome:
   Link:

   We've used concepts of regular expressions, NLP, sentence scores, NLTK, NER, language tools and LLM models.

3. Google Drive upload :
   Used Google Drive API to automate the upload of summarised files to the solicitors' cloud storage.

4. Automated mail sender:
   Automated sending of mail to the solicitors team via python script.

# DEMO 
Legal Document: (INPUT)
1. https://www.bailii.org/ew/cases/EWHC/Costs/2024/1699.html
2. https://www.bailii.org/ew/cases/EWHC/Costs/2024/1600.html
   
Summarised Document: (OUTPUT)
1. https://drive.google.com/file/d/1--7dj6hy8-v_MHDiy2k7smWm2MjJa7vA/view?usp=drivesdk
2. https://drive.google.com/file/d/1-09KBF0nyK5nvwcWa7W47NvJGqwy8UX-/view?usp=drivesdk

