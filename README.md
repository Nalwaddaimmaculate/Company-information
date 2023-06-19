# Company-information
company information and link
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
      
   <title> ARRAY DISPLAY</title>
    </style>


    <script>

let jsondata = [
  {
    "company_name": "Microsoft Corporation",
    "img_src": "https://pbs.twimg.com/profile_images/1645587399479808001/SSEsTaqu_400x400.jpg",
    "about": "Microsoft Corporation, based in Redmond, Washington, is among the world's biggest corporations and ranks first on a list of the Top 10 IT Companies. Microsoft Windows, Microsoft Office, and Internet Explorer, among other products, are used by nearly every business and professional around the world. Microsoft was established in 1975, by Bill Gates and Paul Allen"
  },
  {
    "company_name": "IBM",
    "img_src": "https://pbs.twimg.com/profile_images/1666880941493452802/AN1qCNBw_400x400.jpg",
    "about": "International Business Machines abbreviated as IBM. This is an American multinational company that operates in over 150 countries. The firm began as a computer recording firm before being called IBM (International Business Machines) in 1924. IBM's headquarters are in Armonk, Future York"
  },
  {
    "company_name": "Accenture",
    "img_src": "https://pbs.twimg.com/profile_images/1552786622936129536/JVw0DfVn_400x400.jpg",
    "about": "Accenture is one of the major Information Technology (IT) businesses and is included in the Fortune Global 500. It is a multinational management consulting business that offers professional services such as strategies, consultancy, technologies, and operation."
  },
  {
    "company_name": "Oracle",
    "img_src": "https://pbs.twimg.com/profile_images/1580919426081251330/z11bDhy-_400x400.jpg",
    "about": "Oracle Corporation, one of the top 10 IT companies in the world, is headquartered in Redwood Shores, California, is a well-known American multinational company. With a workforce of around 130,000, Oracle has the second largest revenue in the software development industry after Microsoft."
  },
  {
    "company_name": "SAP",
    "img_src": "https://pbs.twimg.com/profile_images/1664395548823109633/WKlo5STU_400x400.jpg",
    "about": "SAP has effectively established itself as the global leader in corporate application areas of software and software-related operations. SAP is the third biggest software firm by market value, with more than 88,000 professionals in much more than 130 countries. SAP has about 380,000 clients in far more than 170 countries."
  },
  {
    "company_name": "TCS - Tata Consultancy Services",
    "img_src": "https://pbs.twimg.com/profile_images/1542758734501654528/nzNTx_7V_400x400.jpg",
    "about": "Tata Consultancy Services which is abbreviated as TCS. This MNC has been named as one of the leading Indian Multinational Information Technology Corporation, with income generated across multiple areas. TCSs headquarters are in Mumbai, India, and it has numerous functional domains such as consultation systems, software developments, infrastructural support, and business processes outsourcing."
  },
  {
    "company_name": "DXC",
    "img_src": "https://pbs.twimg.com/profile_images/1402623872856465408/nJ48rIIj_400x400.jpg",
    "about": "DXC is an IT services firm that was founded when HPE merged its IT division with CSC. DXC Technology, founded in 2017 as a combination of HPE and CSC, has grown to become one of the world's largest IT firms. As of now, the corporation has broad activities in over 72 nations all over the globe."
  },
  {
    "company_name": "Delloite Consulting",
    "img_src": "https://pbs.twimg.com/profile_images/1539799565016379392/2h4jury3_400x400.png",
    "about": "Deloitte is among the world's leading service companies, serving clients worldwide with services ranging from management consulting to IT technology consulting. Deloitte refers to the chain of member companies of Deloitte Touche Tohmatsu Limited, an organization established in the United Kingdom."
  },
  {
    "company_name": "Capgemini",
    "img_src": "https://pbs.twimg.com/profile_images/1664202032155176961/OmgFdtWj_400x400.jpg",
    "about": "Capgemini is among the world's largest information technology (IT) organizations, with a significant global presence. Capgemini, a French company with its headquarters in Paris, with worldwide functioning in over 42 nations."
  },
  {
    "company_name": "Cognizant",
    "img_src": "https://pbs.twimg.com/profile_images/1664266649304985601/mGLbldKT_400x400.jpg",
    "about": "Cognizant is a major Information technology MNC which helps customers in changing their traditional businesses, operations, and technologies to reap the benefits of quickly altering digital technologies. Thus making it one of the leading IT companies in the world."
  },
  {
    "company_name": "Zensar",
    "img_src": "https://pbs.twimg.com/profile_images/1545016797350744064/Xxt_JFUA_400x400.jpg",
    "about": "Zensar is a technology consulting and services company with 10,000 associates in 33 global locations. More than 130 leading enterprises depend on our expertise to be more disruptive, agile, and competitive."
  }
]
        function getData(){
            
                let str ="<table border='4' class=' table table-responsive'>";
                str = str + "<tr><th> NAME </th> <th> SITE </th> </tr> "
                for(stud of jsondata){
                    //new row begins
                    str=str+"<tr>";
                    for(data in stud ){ 
                        console.log(stud[data]); //one cell
                        let temp = "<td>"+ stud[data] +"</td>";
                        str = str+ temp;
                    }
                    //end row here
                    str=str+"</tr>";


                }
                str = str+"</table>"
                // set it as innerhtml for the div
                document.getElementById('mydiv').innerHTML = str;
        }
    </script>
</head>
<body>
    <style>
    
    
    h1,h2{ /*element selector */
        background-color: aqua;


    }
    /* id selector */
    /* #myspec{
        background-color: bisque;
    } */
    /* #myspec{

    }*/
    .myspec{
        background-color: bisque;

    }
    /* #myspecialdiv{
        background-color: burlywood;
    }*/
    div h1{
        color:beige;
        font-family: Arial, Helvetica, sans-serif;

    }
    #fon{
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        font-weight: bold;
        font-size: 2em;
    }
    #bo{
        border-top: solid 2px blue;
        border-bottom: dashed 3px red;   
    }
    #ech{
        border-top: solid 2px blue;
        border-width: 2px 5px 8px;

    }

 </style>   
    

    <h1> Company information</h1>
    <div id="mydiv"> Table should show here</div>
    <button onclick="getData()"> Click to see data and display</button>


</body>
</html>

