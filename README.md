<h2>This project demonstrates the implementation of a host-based firewall on a Linux system using the iptables utility. The firewall is designed to restrict unauthorized access by blocking traffic from specific IP addresses and denying connections to selected network ports.<h2>
<h2>The goal of this project is to apply foundational cybersecurity principles such as least privilege, default-deny security, and network traffic control in a real-world Linux environment.</h2>
<h2>Here's how i did it. firstly i logged into the root account because i needed root previledges for easy configuration. Then i confirmed the default traffic policies...</h2>



<img width="1792" height="832" alt="image" src="https://github.com/user-attachments/assets/3f6e2b6a-3069-47d8-9548-5c41bbfbff01" />


<h2>The next step was to write the rules i wanted to implement.</h2>


<img width="1792" height="832" alt="image" src="https://github.com/user-attachments/assets/e70c877e-295e-4ae9-a30c-7669ee98eac9" />


<h2>In the first instance i blocked common ports like ssh, ftp and dns. i moved further to block specific ip addresses from connecting to my machine</h2>


<img width="1764" height="484" alt="image" src="https://github.com/user-attachments/assets/f937d5f2-59d0-4d79-966c-4528cf776acc" />


<h2>I blocked tftp and rdp from connecting to my machine from specific ip addreses. i also blocked all incoming traffic from an ip address</h2>


<img width="1732" height="259" alt="image" src="https://github.com/user-attachments/assets/7ca2c675-8005-4c82-adf0-031a570cc75d" />



<h2>What i did next was to block all incoming and outgoing traffic on my machine. (note: this is very dangerous as it effectively disconnects you from the world)</h2>

<img width="1659" height="311" alt="image" src="https://github.com/user-attachments/assets/a07ae037-d538-47c8-9b2a-21b5a23ce663" />



<h2>note: you can also allow specific traffic from the network using the iptables command.</h2>

<h2>after scanning with NMAP and also tryng out the policies i put to be sure it is effective, i flushed the policies i implemented and saved the defualt policy</h2>

<img width="1792" height="832" alt="image" src="https://github.com/user-attachments/assets/a4ceaf68-312a-427e-92cb-601071687924" />


<h2>i succefully flushed and returned it to the default.</h2>

<img width="1792" height="832" alt="image" src="https://github.com/user-attachments/assets/b85550b1-9d65-421a-a86f-668efeebdc35" />


<h2>this project taught me how to use iptables to implement a host-based firewall on Linux, applying least privilege and default-deny principles to control network traffic, block unauthorized IP addresses and ports, and reduce the system’s attack surface in a real-world environment.</h2>



