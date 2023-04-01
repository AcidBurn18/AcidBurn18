<!-- Title -->
<h1 align="center">Hi, I'm Ansh Agrawal 👋</h1>
<!-- About Me -->
<h2>About Me</h2>
<p>I'm a DevOps Engineer with a passion for cloud computing and automation. Currently, I'm working at Hashedin by Deloitte, where I'm responsible for designing and implementing cloud infrastructure for enterprise clients. My experience includes working with various DevOps tools.</p>
<!-- Skills -->
<h2>My Skills</h2>
<ul>
<ul>
  <li><a href="https://www.terraform.io/"><img src="https://img.icons8.com/color/24/000000/terraform.png"/></a> Terraform</li>
  <li><a href="https://cloud.google.com/"><img src="https://img.icons8.com/color/24/000000/google-cloud-platform.png"/></a> Google Cloud Platform (GCP)</li>
  <li><a href="https://azure.microsoft.com/"><img src="https://img.icons8.com/color/24/000000/azure-1.png"/></a> Microsoft Azure</li>
  <li><a href="https://kubernetes.io/"><img src="https://img.icons8.com/color/24/000000/kubernetes.png"/></a> Kubernetes</li>
  <li><a href="https://www.docker.com/"><img src="https://img.icons8.com/color/24/000000/docker.png"/></a> Docker</li>
  <li><a href="https://www.jenkins.io/"><img src="https://img.icons8.com/color/24/000000/jenkins.png"/></a> Jenkins</li>
  <li><a href="https://www.ansible.com/"><img src="https://img.icons8.com/color/24/000000/ansible.png"/></a> Ansible</li>
  <li><a href="https://www.python.org/"><img src="https://img.icons8.com/color/24/000000/python.png"/></a> Python</
</ul>
<!-- Certifications -->
<h2>My Certifications</h2>
    <ul>
  <li style="display:flex;align-items:center">
    <a href="https://www.credential.net/dc4245f0-9c17-427d-b085-61b505ac7ddd">
      <img src="https://api.accredible.com/v1/frontend/credential_website_embed_image/badge/70660985"/>
    </a>
    <a href="https://www.credential.net/309f4179-f9ab-4a34-bcad-7b3ab9854091">
      <img src="https://api.accredible.com/v1/frontend/credential_website_embed_image/badge/67164146" style="margin-left:10px"/>
    </a>
  </li>
</ul>
<!-- Projects -->
<!-- Get In Touch -->
<h2>Get In Touch</h2>
 <div>
  <a href="https://in.linkedin.com/in/gotoansh" style="display:inline-block; margin-right:20px;"><img src="https://img.icons8.com/color/48/000000/linkedin.png"/></a>
  <a href="https://twitter.com/YodaSpokenHas" style="display:inline-block;"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/twitter/twitter-original.svg" alt="Twitter" width="48" height="48"/></a>
</div>
    
<!-- Footer -->
## My Most Used Languages

{% assign total_size = 0 %}
{% for lang in github.languages %}
    {% assign total_size = total_size | plus: lang[1] %}
{% endfor %}

{% for lang in github.languages %}
    {% assign percentage = lang[1] | times: 100.0 | divided_by: total_size %}
    {% capture lang_str %}- {{ lang[0] }}: {{ percentage | round: 1 }}%{% endcapture %}
    {% if forloop.first %}
        {% assign most_used_lang = lang_str %}
    {% else %}
        {% assign most_used_lang = most_used_lang | append: '\n' | append: lang_str %}
    {% endif %}
{% endfor %}

{{ most_used_lang }}

