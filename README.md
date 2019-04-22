# Job-Category-Prediction-on-basis-of-job-details
I was provided different job ids and json files for each id describing company name,job description,etc and was given a csv file mapping json files to their jo category.So my task was to make a job category classifier on basis of job details.
<h3>File details:</h3>
1.data : hass csv file and compressed json files.<br>
2.prepared_data.csv : data prepared after running data_preparation.ipynb<br>
3.data_preparation.ipynb  : for data preparation.<br>
4.Class_ids : job category and class_id mapping.<br>


<h2>Steps to perform this task </h2>
<h3>1.Data Preparation </h3>
I have json files and a csv file telling category for each json file so I went through each json and converted that to text_file attribute for each job id.That text_file attribute has everything relevant for training our model.<br>
Sample:<br>
Trip Store LLP is Travel &amp; Tour Company based out of Mumbai. With a experience of 25 years in the Travel Trade Industry. We are specialized in Customized tours to Destinations across the world.Our approach is different. We don’t plan any trips in advance, instead believe in customizing each trip by designing an ideal itinerary for you. Whether you know precisely where you want to go or need some insight, Trip Store has you covered. We believe in creating a journey that will exceed your expectations. Our passion is to guide you to your dream destination by alleviating the stress for you.Visit our Website- www.tripstore.inComapany Name is Trip Store LLP.Job keywords are operations, tourism, sales,customer, service, travel agency operations, travel agency, holiday packages, tour packages, travel agent activities.Job Industry is Travel / Tourism.Other skills required are customer,service,travel agency operations,travel agency,holiday packages,tour packages,travel agent activities.Job departments are Tour / Travel Management,Back Office Operations.Salary provided is Rs 2.0  - 3.0 Lakh/Yr.Job Description is as follows : &middot; Prior experience in Travel business specifically in Holiday packages&middot; Working in coordination with sales team &amp; suppliers to get quotations and rates&middot; Speaking with suppliers to get the best rates and comparing the quotes by different suppliers&middot; Choosing the best quote and offering the same to sales team or customer&middot; Coordination with account for payment collection of booking&middot; Coordination with ticketing team to get the tickets issue&middot; Coordination with visa team for processing of visa for customers&middot; Handling on tour issues&middot; Taking feedback &amp; testimonials of travelled client.&nbsp;. <br>

Above text is combination of every relevant json keys.<br>
Also mapped job categories to ids.<br>
Class_ids file conatins mapping.Prepared_data.csv file contains data prepared.<br>
<h3>2.Data Cleaning and Text Preprocessing</h3>
 <br> Used google collab and removed irrelevant columns and did text preprocessing like removal of punctuation marks and tokenization,could use stemming and lemmatization but our text does not look so  much in need of that but still will perform that too.</br>
 Then did train and test split.<br>
 
<h3>3.Training Step</h3>
1.Transfer Learning on ULMFiT Architecture(pretrained language model on  Wikitext 103 dataset.<br>



  
  
