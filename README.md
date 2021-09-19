# plotly_project: Improbable Beef (A Study of Bacteria found in Belly Button)

### **Objectives**

The objective of this project is to show the results of a study of bacterial species that have the ability to synthesize proteins that tastes like beef. A food startup company, _Improbable Beef_, wants to synthesize artificial beef that contains micro-organism that tastes like beef. A biological researcher, Rosa, is doing research on finding micro-organism the company is looking for. One hypothesis by Rosa is that the beef tasting bacteria may be found in human naval since a human body is a source of thousands of types of bacteria. Also, different parts of a body harbors different species and a bacteria found in the gut is not the same as the bacteria residing in eyelashes. The bacterial species found in the same body part can also be different from person to person. This is a study of the bacteria found in a person's naval. Rosa's hypothesis is that the ideal bacterial species to make synthetic beef could be found in a person's naval. Rosa collected the bacterial sample found in the belly button of people living across the country. Each person is assigned an anonymous identity number. We helped Rosa build a dashboard (Webpage) that a research participant and a fellow researcher can access. The website will contain the information about the bacterial species found for each person's id, a visual representation of the types of bacteria shown in a bar graph and a bubble chart. There is also a gauge plot to show the frequency of a person washing naval since the results would depend on it.

### **Analysis and Conclusion**

We built a webpage that is both engaging and dynamic using Plotly and bootstrap. The following is a summary of four deliverables for this project. 

### Deliverables 1, 2 and 3

There is a drop down menu that contains the ID number  of each person. Bootstrap is used to resize the display in the browser.  Once the ID is selected, the following things are displayed:
1. The demographic information of the person is displayed. 

2.  A horizontal bar charge is displayed. It contains the information about the top 10 bacterial species OTUs (_Operational Taxonomic Unit_). An OTU number is the ID number a bacteria. There were 80 bacterial types with distinct ID numbers. We plotted the OTUs as a function of *sample_values* which is an array containing the corresponding species name for each bacterial ID number. Some bacteria have different ID numbers, but are clumped under the same *otu_label*. The hover-text is the *otu_lables*. 

3. A bubble  chart displays the the *otu_ids* as the x-axis and the *sample_values* as the y-axis. The marker size is the *sample_values* and the *otu_ids* are the marker colors. The colorscheme used is "Earth". The hover-text is the *otu_lables*. 

4. A gauge chart shows the belly button washing frequency, _wreq_. 


### Deliverable 4

The challenge required us to make three changes in the webpage to make it visually attractive. I made the webpage appearance like a framed tablet. 

1. I added a dark sea green background. 

2. I added a cellpadding of width 50px (50 pixels), a 10% margin-top. I also rounded the corners of the webpage by 20 pixles (*border-radius: 20px*)

3. I added a 20 pixel margin-top between the bubble chart that is full width ("col-md-12") and middle section containing the demographic information/ bar chart/ gauge chart. 

4. An image of a belly is added as the background of the title box of the page using a css-style sheet.