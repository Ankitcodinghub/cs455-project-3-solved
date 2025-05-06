# cs455-project-3-solved
**TO GET THIS SOLUTION VISIT:** [CS455 Project 3 Solved](https://www.ankitcodinghub.com/product/cs455-project-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96323&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS455 Project 3 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

Objective

In this project you will use a “hybrid architecture” (similar to Project2) to create a solution to a problem that require the use of two Machine Learning algorithms. You will use the AWS Rekognition service along with other services.

Description:

Design a system that helps cities use cameras (installed at roads intersections) to catch and bill drivers that commit traffic violations at traffic lights. Such systems are already in use and are likely to be complex and involve challenging problems. However, we will make a few assumptions to make the problem tractable and suitable for a class project.

You can assume the following:

<ul>
<li>The system will be installed in cities and towns in the state of California.</li>
<li>A California license plate number is a combination of 7 characters and digits (A to Z and 0 to 9).
And the state does not allow custom plate numbers. An example California license plate is shown in Figure 1.

Figure 1: Example California license plate: 7 characters long that consist of characters [A to Z] and digits [0 to 9].
</li>
<li>Cameras installed at intersections have Internet access and can communicate with the cloud.</li>
<li>Cities and towns have budget shortfalls and want to save money. They decided not to use
standard mail and stamps for mailing violation nitices. All violations will be delivered to

offenders via text messaging or emails.
</li>
<li>All vehicles drivers have mobile phones and/or email. And this information is in the Department
of Motor Vehicle (DMV) database.
</li>
<li>The DMV database is not in the cloud. It is located in a local network at the state department of
transportation.
</li>
<li>California has a lot of immigrants and international residents. Most speak excellent English, but
a few don’t. It was found that when people don’t understand violation text/emails they tend to
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
ignore them. To increase the rate of collection, text/emails will be sent in the driver’s preferred

communication language (this is also available in the DMV database).

<ul>
<li>The California DMV does not have access to DMV databases of other states. The license plates
of non-California vehicles that are caught violating traffic rules must be placed in a dedicated S3

bucket to be manually processed.
</li>
<li>When a camera detects a traffic violation, it takes a picture of the front or rear of the offending
vehicle. The picture is first sent to an image processing software that extracts the plate from the picture. As far as your system is concerned, you will always get “clean” license plates (Figure 2).
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 2: License plates are extracted out of pictures. This preprocessing happens prior to the plate arriving to your system. Your system only deals with “clean” plates.

• When the camera uploads the picture to the S3 bucket, it adds with the object 3 metadata (as S3 object tags):

</div>
</div>
<div class="layoutArea">
<div class="column">
Tag

Location DateTime

</div>
<div class="column">
Description and Value

Intersection address (e.g., “Main St and 116th AVE intersection, Bellevue”) The date and time the violation took place.

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Type

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
The type of violation. Three types are supported:

 no_stop: vehicle didn’t stop at the red light.

 no_full_stop_on_right: vehicle didn’t come to a full stop before taking

a right on red.

 no_right_on red: right turn on red not allowed.

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
• The type of violation determines the ticket amount the driver must pay:

</div>
</div>
<div class="layoutArea">
<div class="column">
no_stop: no_full_stop_on_right: no_right_on_red:

</div>
<div class="column">
$300.00 $75.00 $125.00

</div>
</div>
<div class="layoutArea">
<div class="column">
• The text message (or email) should have the following format:

Your vehicle was involved in a traffic violation. Please pay the specified ticket amount by 30 days:

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Vehicle: [Color] [Make] [Model]

License plate: [PlateNumber]

Date: [The date/time the violation took place]

Violation address: [Address where the violation took place] Vilation type: [Type of violation]

Ticket amount: [The ticket amount]

Note that only the blue portion needs to be translated to a language other than English. The green portion will always be in English.

For example:

Your vehicle was involved in a traffic violation. Please pay the specified ticket amount by 30 days:

Vehicle: Blue Ford Escort

License plate: BXT7765

Date: 6/12/2021 2:25:47 PM

Violation address: Main St and 116th AVE intersection, Bellevue Vilation type: no_right_on_red

Ticket amount: $125

Build a solution such that when a license plate picture arrives to an S3 bucket, the corresponding vehicle owner is sent a text message or email in his/her preferred language. If a license plate is not a California license plate (e.g., an out of state vehicle), the plate picture must be uploaded to a specific bucket (to be manually processed). Figure 3 shows the system workflow diagram (I also enclosed Figure 3 as a separate PDF in case you want to print it as a guide while working on the project).

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Figure 3: System workflow diagram. Implementation Hints:

<ul>
<li>Some parts of this project have strong resemblance to parts in Project2. Borrow code from your Project2 and fill in the blanks where needed.</li>
<li>The California DMV database is the enclosed DMVDatabase.xml file.
o OpentheenclosedDMVDatabase.xmlfile.

o Changeall5phonenumbersbetween&lt;contact&gt;…&lt;/contact&gt;toyourmobilephone

number. This way you can test the messaging system.
</li>
<li>8 license plates were given to you for testing (see folder LicencePlates). 5 are California plates and 3 are non-California plates.</li>
<li>You can use any AWS service that you like and any programming language. The Lambda roles should contain the policy AmazonRekognitionFullAccess (plus any other policy that you may need).</li>
<li>You may find this function helpful:</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
To use the above function you need to add the following:

<pre>       using System.IO;
       using Amazon.Rekognition.Model;
</pre>
• You may find this function useful:

private bool IsCapitalLettersAndNumbers(string s)

{

if(String.IsNullOrEmpty(s))

{

return false;

}

return System.Text.RegularExpressions.Regex.IsMatch(s, “^[A-Z0-9]*$”); }

Grading rubric:

<ul>
<li>(80 %) You can demo the solution and it works start-to-end (from dropping a license plate into S3 to getting a text message or email).</li>
<li>(20 %) You can explain your code.
What to Submit:

Nothing to submit. You meet with me for 5 minutes and demo your work.
</li>
</ul>
</div>
</div>
</div>
