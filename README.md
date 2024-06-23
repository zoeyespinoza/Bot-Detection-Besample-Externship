# Bot Detection
![Besample](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/https___62e11931a860a39a714f6a6ef2e0a561.cdn.bubble.io_f1673959027254x692225471550134500_B_291x60_color%25201.png)

## Bot Detection for Accurate Survey Results with Besample

Besample is a startup created to help researchers who work in both industry and academia to easily study diverse people from across the globe. they aim to enhance the reliability and accuracy of its survey results. Given the prevalence of automated bots that can skew data integrity, it is essential to identify and filter out these non-human participants. The presence of bots not only affects the authenticity of the survey data but also compromises the quality of insights derived from the research. Consequently, BeSample is committed to employing machine learning techniques to detect and mitigate the impact of bots on their surveys.

[Besample's website](https://besample.app/)

[Presentation Slides](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/Besample_PresentationSlides.pdf)
## Purpose
![slide](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/slide4.jpg)
The primary goal of this project is to develop a robust machine learning model that can efficiently identify bots within the user base. 
By achieving this, BeSample aims to:

**Enhance Data Integrity:** Ensure that survey results are exclusively derived from genuine respondents.

**Improve Survey Quality:** Increase the reliability of insights and decisions made based on survey data.

**Optimize Resource Allocation:** Reduce wasted resources on processing and analyzing responses.

## Bot Activity
![Bot Activity over Time](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/botactivityovertime.png)

To look for bots, we can look for anomalies or inconsistencies in response times, patterns in answers, IP addresses, and existing flags. 
- Check for unusual patterns such as identical response times across different surveys. 
- Look for non-diverse IP addresses or multiple from the same IP in a short timeframe. 
- Analyze response patterns for uniformity that might indicate scripted (Bot-like) answers.

The 'isBot' column can be a lead for indicating Bot-like behavior. This column was created after an attack Mid January 2024. However, the company said these values were quickly assigned and may not be correct.
#EDA and Analysis
![slide](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/ip.png)
![slide](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/duration.png)
![slide](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/correlational_analysis.png)


Flagging the hard facts and soft facts for potenttial bots and suspicious users, in the multiple columns revelaed: 
![slide](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/slide9.jpg)

![slide](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/slide11.jpg)
![slide](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/slide10.jpg)

## Conclusions

Flagging the hard facts and soft facts for potenttial bots and suspicious users, in the multiple columns revelaed: 

**380 suspicious users**

**71 matched with the 'isBot' column**
![match](https://github.com/zoeyespinoza/Bot-Detection-Besample-Externship/blob/main/graphs/isbot%20match.png)

### Suggestions for Future Proofing

- Employ Two-Factor Authentication
- Automate unique survey links for participants to prevent bots from accessing multiple surveys with the same link.
- Include hidden items in a survey that will be seen by computers but not by respondents, so if completed it will flag as bot (honeypot).
- Apply rate limiting, IP address monitoring services, security (Cloudflare).
- Use third-party bot detection services or APIs.
- Utilize machine learning algorithms to continuously improve bot detection capabilities and stay ahead of threats.



