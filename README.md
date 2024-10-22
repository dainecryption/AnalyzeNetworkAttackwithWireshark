<h1>Analyze Network Attack with Wireshark</h1>

<h2>Scenario</h2>

<i>This scenario is based on a fictional event.</i>

I work as a security analyst for a travel agency that advertises sales and promotions on the company’s website. The employees of the company regularly access the company’s sales webpage to search for vacation packages their customers might like. 

One afternoon, I received an automated alert from my monitoring system indicating a problem with the web server. I attempted to visit the company’s website, but I received a connection timeout error message in my browser.

I used a packet sniffer to capture data packets in transit to and from the web server. I noticed a [large number of TCP SYN requests coming from an unfamiliar IP address](https://github.com/dainecryption/AnalyzeNetworkAttackwithWireshark/blob/main/Wireshark%20TCP_HTTP%20log.pdf). The web server appears to be overwhelmed by the volume of incoming traffic and is losing its ability to respond to the abnormally large number of SYN requests. I suspected the server is under attack by a malicious actor. 

I took the server offline temporarily so that the machine can recover and return to a normal operating status. I also configured the company’s firewall to block the IP address that was sending the abnormal number of SYN requests. I know that my IP blocking solution won’t last long, as an attacker can spoof other IP addresses to get around this block. I needed to alert my manager about this problem quickly and discuss the next steps to stop this attacker and prevent this problem from happening again. I will need to be prepared to tell my boss about the type of attack I discovered and how it was affecting the web server and employees through a [cybersecurity incident report](https://github.com/dainecryption/AnalyzeNetworkAttackwithWireshark/blob/main/AnalyzeNetworkAttackwithWireshark.pdf).

<br />
