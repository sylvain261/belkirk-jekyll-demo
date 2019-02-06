---
title: Home
banner_image: "/img/banner.png"
layout: landing-page
heading: Belkirk College
partners:
- "/uploads/2017/11/13/stem.png"
- "/uploads/2017/11/13/UPenn_logo.png"
- "/uploads/2017/11/13/nysed.png"
services:
- description: Performing collaborative research and providing services to support
    the Health Sector.
  heading: Health
  icon: "/uploads/2017/11/13/health.png"
- description: Performing collaborative research and providing services to support
    the biotechnology sector.
  heading: BioTech
  icon: "/uploads/2017/11/13/biotech.png"
sub_heading: Engineering and Health Sciences
textline: "<div class=\"overlay\">\n\n\t\t\t\n\n\t\t<p>\n\n\t\t\t<span class=\"nbr\">01</span>\n\n\t\t\tRun
  <strong>list-certificates</strong> command (OSX/Linux/UNIX) using built-in query
  filters to list all issued SSL/TLS certificates managed by AWS ACM service, available
  in the selected region:\n\n</p><div class=\"code-container\">\n\n\t<div class=\"nbrs-row\"><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span><span>32</span><span>33</span><span>34</span><span>35</span><span>36</span><span>37</span><span>38</span><span>39</span><span>40</span><span>41</span><span>42</span><span>43</span><span>44</span><span>45</span><span>46</span><span>47</span><span>48</span><span>49</span></div>\n\n\t<pre>aws
  acm list-certificates\n\n\t--region us-east-1\n\n\t--certificate-statuses ISSUED\n\n</pre>\n\n</div>\n\n\t\t<p></p>\n\n\t\t<p>\n\n\t\t\t<span
  class=\"nbr\">02</span>\n\n\t\t\tThe command output should return the metadata (domain
  name and ARN) for all issued (validated) AWS ACM certificates currently available
  in the US East (N. Virginia) region:\n\n</p><div class=\"code-container\">\n\n\t<div
  class=\"nbrs-row\"><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span><span>32</span><span>33</span><span>34</span><span>35</span><span>36</span><span>37</span><span>38</span><span>39</span><span>40</span><span>41</span><span>42</span><span>43</span><span>44</span><span>45</span><span>46</span><span>47</span><span>48</span><span>49</span></div>\n\n\t<pre>{\n\n
  \   \"CertificateSummaryList\": \\[\n\n        {\n\n            \"CertificateArn\":
  \"arn:aws:acm:us-east-1:1234567890:\n\n             certificate/F1c6999d-b027-4449-9694-55ce71b3655C\",\n\n
  \           \"DomainName\": \"cloudconformity.com\"\n\n        }\n\n    \\]\n\n}\n\n</pre>\n\n</div>\n\n\t\t<p></p>\n\n\t\t<p>\n\n\t\t\t<span
  class=\"nbr\">03</span>\n\n\t\t\tRun <strong>describe-certificate</strong> command
  (OSX/Linux/UNIX) using the ARN of the certificate returned at the previous step
  as identifier and custom query filters to return the timestamp (UNIX format) of
  the expiration date for the selected certificate:\n\n</p><div class=\"code-container\">\n\n\t<div
  class=\"nbrs-row\"><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span><span>32</span><span>33</span><span>34</span><span>35</span><span>36</span><span>37</span><span>38</span><span>39</span><span>40</span><span>41</span><span>42</span><span>43</span><span>44</span><span>45</span><span>46</span><span>47</span><span>48</span><span>49</span></div>\n\n\t<pre>aws
  acm describe-certificate\n\n\t--region us-east-1\n\n\t--certificate-arn arn:aws:acm:us-east-1:1234567890:certificate/F1c6999d-b027-4449-9694-55ce71b3655C\n\n\t--query
  'Certificate.NotAfter'\n\n</pre>\n\n</div>\n\n\t\t<p></p>\n\n\t\t<p>\n\n\t\t\t<span
  class=\"nbr\">04</span>\n\n\t\t\tThe command output should return the timestamp
  of the expiration date for the selected certificate:\n\n</p><div class=\"code-container\">\n\n\t<div
  class=\"nbrs-row\"><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span><span>32</span><span>33</span><span>34</span><span>35</span><span>36</span><span>37</span><span>38</span><span>39</span><span>40</span><span>41</span><span>42</span><span>43</span><span>44</span><span>45</span><span>46</span><span>47</span><span>48</span><span>49</span></div>\n\n\t<pre>1490140799\n\n</pre>\n\n</div>\n\n\t\t<p></p>\n\n\t\t<p>\n\n\t\t\t<span
  class=\"nbr\">05</span>\n\n\t\t\tNow run <strong>date</strong> command (Linux/UNIX)
  using the timestamp value returned at the previous step to convert it to a human
  readable date value:\n\n</p><div class=\"code-container\">\n\n\t<div class=\"nbrs-row\"><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span><span>32</span><span>33</span><span>34</span><span>35</span><span>36</span><span>37</span><span>38</span><span>39</span><span>40</span><span>41</span><span>42</span><span>43</span><span>44</span><span>45</span><span>46</span><span>47</span><span>48</span><span>49</span></div>\n\n\t<pre>date
  -d @1490140799\n\n</pre>\n\n</div>\n\n\t\t<p></p>\n\n\t\t<p>\n\n\t\t\t<span class=\"nbr\">06</span>\n\n\t\t\tThe
  command output should return the requested date in human readable format (UTC time):\n\n</p><div
  class=\"code-container\">\n\n\t<div class=\"nbrs-row\"><span>1</span><span>2</span><span>3</span><span>4</span><span>5</span><span>6</span><span>7</span><span>8</span><span>9</span><span>10</span><span>11</span><span>12</span><span>13</span><span>14</span><span>15</span><span>16</span><span>17</span><span>18</span><span>19</span><span>20</span><span>21</span><span>22</span><span>23</span><span>24</span><span>25</span><span>26</span><span>27</span><span>28</span><span>29</span><span>30</span><span>31</span><span>32</span><span>33</span><span>34</span><span>35</span><span>36</span><span>37</span><span>38</span><span>39</span><span>40</span><span>41</span><span>42</span><span>43</span><span>44</span><span>45</span><span>46</span><span>47</span><span>48</span><span>49</span></div>\n\n\t<pre>Tue
  Mar 21 23:59:59 UTC 2017\n\n</pre>\n\n</div>\n\n<br>\n\nIf the date returned is
  30 days from the checkup date, the selected SSL/TLS certificate is about to expire
  and should be renewed soon (see Remediation/Resolution section for the renewal process).\n\n\t\t<p></p>\n\n\t\t<p>\n\n\t\t\t<span
  class=\"nbr\">07</span>\n\n\t\t\tRepeat steps no. 3 – 6 to check other SSL/TLS certificates
  that are about to expire soon, managed by AWS ACM within the current region.\n\n\t\t</p>\n\n\t\t<p>\n\n\t\t\t<span
  class=\"nbr\">08</span>\n\n\t\t\tChange the AWS region by updating the<strong> --region</strong>
  command parameter value and repeat the entire audit process for other regions.\n\n\t\t</p>\n\n\t\t\n\n\t\t</div>"
hero_button:
  text: Learn more
  href: "/about"
show_news: true
show_staff: false
aaaa: ''
block1: []
md: ''
menu:
  navigation:
    identifier: _index
    weight: 1

---
