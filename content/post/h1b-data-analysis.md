---
date: 2017-04-09T10:58:08-04:00
featured_image: "/images/clouds.jpg"
tags: ["data analysis", "visualization", "plotly", "python"]
title: "H1B Data Analysis"
---

In recent years, there are a lot of heated debates on whether H-1B visa program is good or bad for America. Considering this visa program only grants 85,000 foreign employees each year and the total employed in the US is 146,624,000 in 2017, it is interesting to see how the 0.058% workforce has generated such strong responses from both sides. 

While news such as [Disney forced 250 its IT employees to train up their foreign replacement before their layoff](https://www.nytimes.com/2015/06/04/us/last-task-after-layoff-at-disney-train-foreign-replacements.html) or [how a former Microsoft employee denied H-1B went home and started a $7 billion company](https://money.cnn.com/2017/02/02/news/india/snapdeal-india-kunal-bahl-h1b-visa/index.html) probably cannot tell the whole story, unsensational data may tell us more.

## H-1B General Trend

The number of H-1B applicants has been increasing since 2010, after the Great Recession. But, this trend has stopped in 2017. This is quite interesting, since the economy has been doing great and the total employed number in the United States has been increasing. See the following two plots. Does it have anything to do the current political atmosphere? One can only guess :-)

<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<div id="7ed07c9c-981c-4584-a383-11e76c7d07c4" style="height: 200; width: 300;" class="plotly-graph-div"></div><script type="text/javascript">window.PLOTLYENV=window.PLOTLYENV || {};window.PLOTLYENV.BASE_URL="https://plot.ly";Plotly.newPlot("7ed07c9c-981c-4584-a383-11e76c7d07c4", [{"type": "scatter", "x": [2013, 2014, 2015, 2016, 2017], "y": [442277, 519504, 618804, 647852, 624650], "mode": "lines+markers", "name": "H-1B"}, {"type": "scatter", "x": [2013, 2014, 2015, 2016, 2017], "y": [44152, 70998, 88994, 126143, 97603], "mode": "lines+markers", "name": "PERM"}], {}, {"showLink": true, "linkText": "Export to plot.ly"})</script>

<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<div id="0d4d5776-63aa-45e4-a5e5-60cad6a61245" style="height: 200; width: 300;" class="plotly-graph-div"></div><script type="text/javascript">window.PLOTLYENV=window.PLOTLYENV || {};window.PLOTLYENV.BASE_URL="https://plot.ly";Plotly.newPlot("0d4d5776-63aa-45e4-a5e5-60cad6a61245", [{"type": "scatter", "x": [2013, 2014, 2015, 2016, 2017], "y": [136369, 138936, 141818, 144348, 146624], "mode": "lines+markers"}], {}, {"showLink": true, "linkText": "Export to plot.ly"})</script>


## Who Are the Biggest H-1B Sponsors?

You may guess that companies who filed the most H-1B applications are big tech companies. After all, this visa is intended to hire foreign "specialty" workers when not enough skilled Americans workers can be found. Although tech companies such as Google, Microsoft and Amazon are indeed among the biggest sponsors, You may be shocked to find out US companies only file about 30% of applications among the Top 15 biggest sponsors.The following table details the Top 15 biggest H-1B sponsors in 2017. The pie chart shows a breakdown of country of headquarters for the top 15.


H-1B Sponsor Name | Number of Application | Headquarter
------------- |-------------:|-------------:
INFOSYS LIMITED | 20587 | India
TATA CONSULTANCY SERVICES LIMITED | 13529 | India
CAPGEMINI AMERICA INC | 9604 | France
IBM INDIA PRIVATE LIMITED | 8734 | India
TECH MAHINDRA (AMERICAS),INC. | 7543 | India
DELOITTE CONSULTING LLP | 7179 | US
ACCENTURE LLP | 6690 | Ireland
ERNST & YOUNG U.S. LLP | 6096 | US
WIPRO LIMITED | 5177 | India
GOOGLE INC. | 5074 | US
MICROSOFT CORPORATION | 5005 | US
HCL AMERICA, INC. | 4263 | India
SYNTEL CONSULTING INC. | 4187 | US
AMAZON CORPORATE LLC | 4165 | US
COGNIZANT TECHNOLOGY SOLUTIONS U.S. CORPORATION | 2707 | US

<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<div id="18b02f35-dd79-43ff-ad0f-f2a7854cbbfc" style="height: 150; width: 150;" class="plotly-graph-div"></div><script type="text/javascript">window.PLOTLYENV=window.PLOTLYENV || {};window.PLOTLYENV.BASE_URL="https://plot.ly";Plotly.newPlot("18b02f35-dd79-43ff-ad0f-f2a7854cbbfc", [{"type": "pie", "labels": ["India", "US", "France", "Ireland"], "values": [59833, 34413, 9604, 6690]}], {"title": "Headquarter Location of Top 15 H-1B Sponsors"}, {"showLink": true, "linkText": "Export to plot.ly"})</script>

If you have read about opinions on how companies like Infosys, Tata Consultancy may be abusing the H-1B visa system and have caused may Americans to lose their jobs, the fact that they are top on the list may not be surprising. The numbers here may make people tempted to blame Indian outsourcing companies for abusing H-1B system. However, there are also France based outsourcing company _Capgemini_ (No. 3), or US based _Syntel_ (No. 13). Well established US companies, such as _IBM_ can create a subsidiary (IBM India Private Limited, No. 4) in another country and embrace outsoursing business model as well. After all, the world is flat.  

In fact, it is probably more interesting to see that only Google, Miscrosoft and Amazon are product companies while the rest of the top 15 are consulting companies.
  
## Most Commom Job Sectors and Mean Wage 
What are the most common occupations among H-1B holders? What are the average wages in each job sector? The following plot can answer those questions. To see the name of the job sector and the number of applicants, hover over each bar in the plot. 


<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<div id="b74f7109-bcb9-4288-b0c2-39c5294681a0" style="height: 200; width: 300;" class="plotly-graph-div"></div><script type="text/javascript">window.PLOTLYENV=window.PLOTLYENV || {};window.PLOTLYENV.BASE_URL="https://plot.ly";Plotly.newPlot("b74f7109-bcb9-4288-b0c2-39c5294681a0", [{"type": "bar", "x": ["15-xxxx", "13-xxxx", "17-xxxx", "11-xxxx", "19-xxxx", "29-xxxx", "25-xxxx", "27-xxxx", "41-xxxx", "23-xxxx", "21-xxxx", "43-xxxx", "39-xxxx", "35-xxxx", "51-xxxx", "53-xxxx", "45-xxxx", "47-xxxx", "31-xxxx", "49-xxxx", "33-xxxx", "37-xxxx", "26-xxxx"], "y": [412440, 47428, 40148, 22078, 21359, 13733, 13352, 7941, 3052, 1907, 1058, 326, 118, 99, 56, 38, 37, 28, 27, 17, 8, 1, 1], "text": ["Computer and Mathematical Occupations", "Business and Financial Operations Occupations", "Architecture and Engineering Occupations", "Management Occupations", "Life, Physical, and Social Science Occupations", "Healthcare Practitioners and Technical Occupations", "Education, Training, and Library Occupations", "Arts, Design, Entertainment, Sports, and Media Occupations", "Sales and Related Occupations", "Legal Occupations", null, null, null, null, null, null, null, null, null, null, null, null, null], "name": "Number of Applications"}, {"type": "scatter", "x": ["15-xxxx", "13-xxxx", "17-xxxx", "11-xxxx", "19-xxxx", "29-xxxx", "25-xxxx", "27-xxxx", "41-xxxx", "23-xxxx", "21-xxxx", "43-xxxx", "39-xxxx", "35-xxxx", "51-xxxx", "53-xxxx", "45-xxxx", "47-xxxx", "31-xxxx", "49-xxxx", "33-xxxx", "37-xxxx", "26-xxxx"], "y": [73195.0, 64376.0, 73715.0, 109117.0, 48277.0, 94702.0, 49250.0, 52707.0, 90768.5, 89107.0, 38917.0, 40456.0, 29682.0, 41891.0, 44013.0, 61610.0, 35672.0, 41683.0, 42702.0, 45573.0, 56222.5, 47611.0, 50794.0], "name": "Average Annual Wage"}], {"title": "Number of Application in Each Job Sector", "xaxis": {"title": "SOC Code"}, "yaxis": {"title": "Number of Applications / Average Annual Wage($)"}}, {"showLink": true, "linkText": "Export to plot.ly"})</script>

## Are H-1B Employees Underpaid?

Many H-1B opponents consider H-1B visas are used by US companies for cheap labors, instead of hiring highly-skilled workers that cannot be find in the US. Let's take a look at the data to see if this is true.

To simplify the analysis, we will only focus on Job Sector `15-xxxx` (Computer and Mathematical Occupations) since about 2/3 of applicants are from this sector. We all know the wage difference even in the same job sector can vary a lot due to the location. For example, according to [Bureau of Labor Statistics](https://www.bls.gov/oes/), for May, 2017, the mean wage for `15-xxxx` in Louisana is $58,510, while it is $100,480 in California. Thus, we will look at median annual wage for H-1B applicants _vs._ the general population state by state. 

<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<div id="738190b6-ae0d-4b0d-9784-22c533fd9075" style="height: 200; width: 300;" class="plotly-graph-div"></div><script type="text/javascript">window.PLOTLYENV=window.PLOTLYENV || {};window.PLOTLYENV.BASE_URL="https://plot.ly";Plotly.newPlot("738190b6-ae0d-4b0d-9784-22c533fd9075", [{"type": "choropleth", "colorscale": "Viridis", "autocolorscale": false, "locations": ["AL", "AK", "AZ", "AR", "CA", "CO", "CT", "DE", "DC", "FL", "GA", "HI", "ID", "IL", "IN", "IA", "KS", "KY", "LA", "ME", "MD", "MA", "MI", "MN", "MS", "MO", "MT", "NE", "NV", "NH", "NJ", "NM", "NY", "NC", "ND", "OH", "OK", "OR", "PA", "RI", "SC", "SD", "TN", "TX", "UT", "VT", "VA", "WA", "WV", "WI", "WY", "GU", "PR", "VI"], "z": [0.7321175409202216, 0.8463541666666666, 0.9211565053425519, 1.0452891287586739, 0.9269705414012739, 0.7875270211846087, 0.7900373599003736, 0.7492780986228343, 0.6450065888554217, 0.9408957722896609, 0.7811790552911022, 0.8169916074887024, 1.0910469150701463, 0.86169881394513, 0.9017950202663578, 0.8800675675675675, 0.9645407428735964, 1.072989122108166, 1.0097846521962057, 0.9465741667858676, 0.679737061769616, 0.8187229437229437, 0.8746663142592838, 0.9161341079641733, 0.9801292407108239, 0.8811916348809681, 1.1148298628745557, 0.9729341641831482, 1.026473844450595, 0.8340280316879951, 0.7149636191078772, 0.8266134580982524, 0.8351472762424657, 0.852567760342368, 1.0275768679305401, 0.8824775185716147, 0.8405817174515235, 0.8975524475524476, 0.8936243318910664, 0.9233669548511048, 0.846642228739003, 0.9355966050923614, 0.9270102651839178, 0.8173723829687133, 0.8549399815327793, 1.2208158844765342, 0.7270048259574905, 0.8625143733231123, 0.9648156937193482, 1.0077845982142857, 0.8292480953958264, 0.9056003486598387, 1.214923076923077, 1.0402014098690835], "locationmode": "USA-states", "text": ["AL<br>state-wide: 77590<br>H-1B: 56805.0", "AK<br>state-wide: 76800<br>H-1B: 65000.0", "AZ<br>state-wide: 79550<br>H-1B: 73278.0", "AR<br>state-wide: 64850<br>H-1B: 67787.0", "CA<br>state-wide: 100480<br>H-1B: 93142.0", "CO<br>state-wide: 92520<br>H-1B: 72862.0", "CT<br>state-wide: 88330<br>H-1B: 69784.0", "DE<br>state-wide: 90040<br>H-1B: 67465.0", "DC<br>state-wide: 106240<br>H-1B: 68525.5", "FL<br>state-wide: 71670<br>H-1B: 67434.0", "GA<br>state-wide: 81930<br>H-1B: 64002.0", "HI<br>state-wide: 77450<br>H-1B: 63276.0", "ID<br>state-wide: 66290<br>H-1B: 72325.5", "IL<br>state-wide: 83470<br>H-1B: 71926.0", "IN<br>state-wide: 69080<br>H-1B: 62296.0", "IA<br>state-wide: 74000<br>H-1B: 65125.0", "KS<br>state-wide: 69460<br>H-1B: 66997.0", "KY<br>state-wide: 65270<br>H-1B: 70034.0", "LA<br>state-wide: 58510<br>H-1B: 59082.5", "ME<br>state-wide: 69910<br>H-1B: 66175.0", "MD<br>state-wide: 95840<br>H-1B: 65146.0", "MA<br>state-wide: 92400<br>H-1B: 75650.0", "MI<br>state-wide: 75670<br>H-1B: 66186.0", "MN<br>state-wide: 82620<br>H-1B: 75691.0", "MS<br>state-wide: 61900<br>H-1B: 60670.0", "MO<br>state-wide: 76030<br>H-1B: 66997.0", "MT<br>state-wide: 59070<br>H-1B: 65853.0", "NE<br>state-wide: 73820<br>H-1B: 71822.0", "NV<br>state-wide: 72260<br>H-1B: 74173.0", "NH<br>state-wide: 82050<br>H-1B: 68432.0", "NJ<br>state-wide: 94830<br>H-1B: 67800.0", "NM<br>state-wide: 72670<br>H-1B: 60070.0", "NY<br>state-wide: 87930<br>H-1B: 73434.5", "NC<br>state-wide: 84120<br>H-1B: 71718.0", "ND<br>state-wide: 62770<br>H-1B: 64501.0", "OH<br>state-wide: 76730<br>H-1B: 67712.5", "OK<br>state-wide: 64980<br>H-1B: 54621.0", "OR<br>state-wide: 82940<br>H-1B: 74443.0", "PA<br>state-wide: 78580<br>H-1B: 70221.0", "RI<br>state-wide: 83280<br>H-1B: 76898.0", "SC<br>state-wide: 68200<br>H-1B: 57741.0", "SD<br>state-wide: 60090<br>H-1B: 56220.0", "TN<br>state-wide: 70140<br>H-1B: 65020.5", "TX<br>state-wide: 85020<br>H-1B: 69493.0", "UT<br>state-wide: 75810<br>H-1B: 64813.0", "VT<br>state-wide: 69250<br>H-1B: 84541.5", "VA<br>state-wide: 97390<br>H-1B: 70803.0", "WA<br>state-wide: 104360<br>H-1B: 90012.0", "WV<br>state-wide: 63210<br>H-1B: 60986.0", "WI<br>state-wide: 71680<br>H-1B: 72238.0", "WY<br>state-wide: 60380<br>H-1B: 50070.0", "GU<br>state-wide: 45890<br>H-1B: 41558.0", "PR<br>state-wide: 39000<br>H-1B: 47382.0", "VI<br>state-wide: 49650<br>H-1B: 51646.0"], "marker": {"line": {"color": "rgb(255,255,255)", "width": 1}}, "colorbar": {"title": "h1b/state ratio"}}], {"title": "Wage Ratio (h1b/state) Among Computer and Mathematical Occupations<br>(Hover for breakdown)", "geo": {"scope": "usa", "projection": {"type": "albers usa"}, "showlakes": true, "lakecolor": "rgb(255, 255, 255)"}}, {"showLink": true, "linkText": "Export to plot.ly"})</script>

The data shows that in the majority of the states, H-1B workers are underpaid. 

When I was studying on the topic, I come aross [this article](https://www.glassdoor.com/research/h1b-workers/) by Andrew Chamberlain, the Chief Economist of Glassdoor. Based Glassdoor users' self-reported data, H-1B workers actually make more in studied job categories in Top 10 cities in the US.

This is an interesting result and my theory is that employees in outsourcing companies are less inclined to report their salary on Glassdoor. Think about this, assume that you are a H-1B worker from Bangalore, India and temporarily doing consulting work in Boston this quarter and will be working in Chicago next quarter. Considering Glassdoor has only about 486,300 salary data in India currently and it is less prominent in India than the US, would you even know of Glassdoor.  When you use Glassdoor, would you consider you are based in Bangalore, or Boston, or Chicago? There is a high possibility that foreign workers working for an out-sourcing companies are not familier with Glassdoor. If they do, it is more likely for them to report their location as where they are from. It will be very interesting to look more into this.


## Where Did You Get Your Data?
I stumble across the company [Enigma](https://www.enigma.com/) and I'm very impressed with their public data collection. I have used their data in U.S. Federal Government ==> Department of Labor ==> Office of Foreign Labor Certification, where they have H-1B Visa Application data from 2006 to 2017. I also get a few data sets from [Bereau of Labor Statistics](https://www.bls.gov/) for comparison analysis. (e.g. US employment data, US wage data by job sector and state). If you are interested in the exact links to the datasets and the Python script I used, feel free to take a look at the [h1b_analysis project](https://github.com/kuol/h1b_analysis) on my GitHub.   
