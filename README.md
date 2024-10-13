
# HR Analysis Dashboard

A brief description of what this project does and who it's for

# HR Analysis-Dashboard

### Dashboard Link :https://app.powerbi.com/groups/me/reports/e5b8c3ef-e9fa-4fc5-a075-f5c466811e3b/ReportSection814d30b92950be89816e?experience=power-bi

## Problem Statement

Developed a Power BI project focused on HR Data for a company facing challenges in comprehending their employee data to extract valuable insights.Constructing a comprehensive dashboard that includes the following components

Summary page:
- presenting a page of Key HR metrics
### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a Excel file.
- Step 2 : created Background page  To calculate a total employee Headcount -By Using card ,drag and drop the EEID . Right click and select count option.To remove the text , turn off category label.setting border as rounded corner.Insert an image to indicate total headcount employees
- Step 3 : Showcase Year-on-Year trends Headcount & Attrition-Click on line graph and select hire date and click on year under this drag and drop to x-axis. drag and drop employee id to  Y axis and right click select count .To show case values select visual-> enable data label.select the font and color. format Xaxis and Yaxis values. To remove the grid lines, Go to Grid line ->Horizantal & Vertical -turnoff.change the title as Employee Headcount Volume trend and format the title change the color.
- Step 4 : To display gender wise split,add a donut chart,drag and drop gender to legend.employee id drag and drop the values.Set the border corner as rounded corner(10).set the background color
- Step 5 : Headcount distribution across various age groups - By using cluster bar chart,drag and drop Employee id into X axis,age into Y axis.change the type into categorical in Y axis to change the view.To sort the age , click on three dots, select sort--> Age. Then we have a clear view.change the title as Employee Headcount volume by age group.
- Step 6 : Breakdown of Headcount by country- By using Decomposition tree ,drag and drop count of country into analyze,country into explain by, then change the format -->density--> dense. Format the values and gave the title as Headcount by Country'
- Step 7 : Analyze Headcount based on Business Unit - By using tree map,drag and drop business unit into category and Employee id count into values. go to format , turn on data labels to show the values and set the font size for values.Go to Category labels set the font size for text.
- Step 8 : Break down of Headcount by Employee Designation - By using cluster bar chart, drag and drop job title into category and employee Id into values. Go to General and format the Yaxis (set the font, size and color).Format the Xaxis- set the font , size and color.Change the title as employee headcount by Designation
- Step 9 : To Calculate Gender wise count, using Dax function. clicking on Measure tools-->New Measure.
Total_Count = CountA('Empolyee Data '[Gender]) 
Total_Male_count = COUNTAX(FILTER'EMPLOYEE DATA'[GENDER]="MALE",'EMPLOYEE DATA'[EEID])
Total_FEMALE_count = COUNTAX(FILTER'EMPLOYEE DATA'[GENDER]="FEMALE",'EMPLOYEE DATA'[EEID]) 
step 10: create a rounded corner shape, and add a female & male image into this shape, drag and drop male and female head count near by image.
step 11: To calculate a male and female Percentange,         
Male % = DIVIDE(Total_Male_count),[TOTALCOUNT])
Female % = DIVIDE(Total_Female
_count),[TOTALCOUNT])
Change the format as percentage and drag and drop the values near by male and feamle image and change the number as without decimal.
- step 11: Insert a shape and add a title as HR HC Analysis Dashboard
- step 12: Insert left and right arrow to indicate the female and male headcount
- step 13: Insert a slicer and drag and drop the Business Unit and format the text and underline the header.If I select the sales option , It will show the sales data only.set the basckground as 100% transparency.
- step 14: Insert a slicer based on country.drag and drop the country.If I selct US, It will display US data only.If I select HR in Business Unit and United States in Country, it will reflect the data in dashboard.
- step 15: Insert a slicer , drag and drop the Full Name.It is more than 3. So we select format-->slicer settings-->options-->style-->instead of vertical list select dropdown.
- step 16: Insert a slicer, drag and drop the Hire date, select instead of drop down, select Between and format the font size , and add a title as Date.
- step 17: click on hometab -->transform data-->New source-->Blank Query-->=Datetime.LocalNow()
It will display the date and time . Then click on To Table --> To Table . We can see current date and time in table.then click on column change the name as Last Refresh. Then click on close and apply.We can see the Query in our dashboard.
- step 18: click on card . select Query1--> last Refresh drag and drop into this card.format the date and time by changing font size and turn off category label.If We want date only , New Measure-->Date = Format(Query1[Last Refresh],"MM/DD/YYYY") Click on tick mark, select Name --> Date, Date type-->Date, format --> short date, drag and drop the Date.
change the border as rounded corner and set the transparency
- step 19: To reset the filter or to create a bookmark, insert an filter image, then go to view tab-->bookmark-->click on add-->call home page,then click on bookmark image, go to format-->actions-->type-->select bookmark, go to bookmark-->home page.If I select multiple filters like IT, US , Then I want to clear the filter , ctrl+click filter image , it will reset.
- step 20: To display attrition , click on employee headcount card, secondary yaxis--> End date -->count. change the name as Attrition count. to set bottom Right , go to format-->visual-->position --> bottom center . click on secondary Yaxis-->minimum-0 & Maximum-->50
- step 21 : To export the attrition data, click on table , add the data whatever needed,  For Ex, Employee full name,hire date, end date and add the border to all the slicer.

 Create a Summary Page :
 - step 22: create a new page in power bi. go to powerpoint, blank presentation. right click -->layout-->blank. Then click on format background-->solid fill-->purple color 
then click on shapes-->rounded rectangle, change the background as white. add the rectangle shape into bottom right corner to hide the color and give no border.Insert a rectangle shape into this and assign a light grey background color. Insert 4 square into it. and and a rectangle into center.click on shapes -->rounded rectangle, go to shape effects-->preset change the background color as dark grey.Insert the text as HR Dashboard Overview, go to shape format-->text effects-->glow change the color as blue.
- step 23: insert calendar icon into first square. insert data source image into second square, Insert refresh icon into third square. Insert mail icon into 4th square.Insert overview icon into center shape. click on snipping tool and save as an image.Insert this image into power bi .Then Insert buttons-->blank --> style -->default go to text -->frequency and format the text and remove the border.Likewise create overview, Refresh, Contact, Data source.
- step 24: Likewise create HR summary go to -->actions-->type--> Page Navigation. select destination-->HR Dashboard.
- step 25: create a shape into frequency columnand named as Every Friday and remove the border. Likewise In datasource we mention as Excel. In Last refreh column,add the date query, date time added to this card .In contact, add the emailid.
- step 26: create HR Analysis . actions --> type--> page Navigation, select destination-->HR Dashboard



