Download Link: https://assignmentchef.com/product/solved-cloud-computing-lab-5-load-balancing
<br>
<h2>Load Balancing</h2>

Dear Happy Vacationer

<ul>

 <li>The previous experiment was so easy that I’m ashamed to even talk about it</li>

 <li>Now you need to do one large experiment that worths a two-week time</li>

 <li>This is load balancing</li>

</ul>

<h2>Goal for Lab 5</h2>

<ul>

 <li>Objectives:</li>

 <li>Understanding the concept of load balancing</li>

 <li>Monitor the utilization status of each VM and each host</li>

 <li>Moving VMs from hot spot to cold ones</li>

 <li>Complete this experiment using at least two computers, the more the better</li>

</ul>

<h2>To Start</h2>

<ul>

 <li>Go to dockerhub and pull one image call mongo-express</li>

 <li><a href="https://hub.docker.com/_/mongo-express">https://hub.docker.com/_/mongo</a><a href="https://hub.docker.com/_/mongo-express">–</a><a href="https://hub.docker.com/_/mongo-express">express</a></li>

 <li>Test this mongodb web service with simple SQL statement</li>

 <li>Hints, you can generate your own DB file on random data</li>

 <li>Write a HTTP request generator that wraps SQL statement</li>

 <li><a href="https://sourceforge.net/projects/http-req-gen/">https://sourceforge.net/projects/http</a><a href="https://sourceforge.net/projects/http-req-gen/">–</a><a href="https://sourceforge.net/projects/http-req-gen/">req</a><a href="https://sourceforge.net/projects/http-req-gen/">–</a><a href="https://sourceforge.net/projects/http-req-gen/">gen/</a></li>

 <li>https://github.com/Kong/httpsnippet</li>

</ul>

<h2>Combine Them Up</h2>

<ul>

 <li>First, connect your request generator to the MongoDB service, basically shooting different SQL statement at a self-defined rate</li>

 <li>Second, make multiple duplicates of the MongoDB service, and randomly distribute the SQL statement to all service hosts</li>

 <li>Third, based on your homework 2-3, use your hypercall to detect the runtime system status, including CPU utilization, memory utilization, etc.</li>

 <li>Set a threshold for such status and name it as the hotspot when it is over</li>

 <li>g., when CPU util &gt; 80%, this is a hot spot, you need to either move some hosts to other machines, or distribute less workloads to this spot</li>

</ul>