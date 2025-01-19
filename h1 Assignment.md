# h1 Asssignment

## Summaries
### Threat Modeling

#### Braiterman et al 2020: Threat Modeling Manifesto

-Focus on people and simplicity.
-Threat modeling is an ongoing process, not a one-time event.
-Collaboration between different teams is critical.
-Models should align with business goals and remain adaptable.
-Question: How can companies simplify models while addressing complex threats?

#### Shostack 2022: Welcome to the World's Shortest Threat Modeling Course

-Introduces four key questions:
 -What are we building?
 -What can go wrong?
 -What are we doing about it?
 -Did we do a good job?
-Visual tools like data flow diagrams help understand systems.
-Threat modeling should improve over time.
-Idea: Integrate threat modeling into weekly team discussions for better awareness.

#### OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet

-Start with simple steps and update models regularly.
-Document decisions for transparency.
-Use techniques like STRIDE and attack trees to find risks.
-Question: How can a small company with no dedicated security team use OWASP’s advice effectively?

### Infosec Scene
#### Darknet Diaries Podcast Episode: Example: "The Beirut Bank Job"

-A real-world case of cyberattacks on banks in the Middle East.
-Shows how political motives drive advanced persistent threats (APTs).
-Highlights human error and phishing as key attack points.
-Question: How can international politics influence cybersecurity strategies?

### Security Hygiene
#### Basic security steps for everyone and businesses:

-Use strong, unique passwords and a password manager.
-Turn on multi-factor authentication (MFA).
-Keep devices, apps, and systems updated (apply patches quickly).
-Use secure connections like HTTPS or VPNs.
-Train people to avoid phishing (e.g., don’t click on suspicious links).
-Back up data regularly and test recovery processes.
-Only give access to people who need it (least privilege).
-Install antivirus and anti-malware tools.

### Make-Belief Boogie-Man: Threat Model for an Imaginary Company
#### Fake Company: Cloudly Designs
A SaaS company providing online graphic design tools.

#### (1) What are we building?
-Important Assets:

 -Customer design files and data (most valuable).
 -Proprietary design algorithms and intellectual property.
 -Login and payment information.
 -Internal tools used by employees for development and support.

-How Customers Use It:

 -Through a website or mobile app.
 -APIs to connect with other tools.
 -A customer support site.

-Diagram: [Uploading h1.<mxfile host="app.diagrams.net" agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/131.0.0.0 Safari/537.36" version="24.7.16">
  <diagram name="Page-1" id="N1R2GWHGTFnKWPwAfik7">
    <mxGraphModel dx="794" dy="458" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="syKNFbUEqoHMrX5vQTZi-1" value="" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="120" y="40" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-3" value="" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="120" y="160" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-4" value="" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="120" y="280" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-5" value="" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="320" y="160" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-6" value="" style="rounded=1;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="520" y="160" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-7" value="Third Party Services (Payments/Analytics)" style="text;html=1;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;" vertex="1" parent="1">
          <mxGeometry x="145" y="55" width="70" height="30" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-8" value="Backend Servers" style="text;html=1;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;" vertex="1" parent="1">
          <mxGeometry x="150" y="175" width="60" height="30" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-9" value="Cloud Storage" style="text;html=1;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;" vertex="1" parent="1">
          <mxGeometry x="150" y="295" width="60" height="30" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-10" value="Websites/Apps" style="text;html=1;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;" vertex="1" parent="1">
          <mxGeometry x="350" y="175" width="60" height="30" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-12" value="Customers" style="text;html=1;align=center;verticalAlign=middle;whiteSpace=wrap;rounded=0;" vertex="1" parent="1">
          <mxGeometry x="550" y="175" width="60" height="30" as="geometry" />
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-13" value="" style="endArrow=classic;html=1;rounded=0;exitX=0;exitY=0.5;exitDx=0;exitDy=0;entryX=1;entryY=0.5;entryDx=0;entryDy=0;" edge="1" parent="1" source="syKNFbUEqoHMrX5vQTZi-5" target="syKNFbUEqoHMrX5vQTZi-3">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="380" y="270" as="sourcePoint" />
            <mxPoint x="430" y="220" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-14" value="" style="endArrow=classic;html=1;rounded=0;exitX=0;exitY=0.5;exitDx=0;exitDy=0;entryX=1;entryY=0.5;entryDx=0;entryDy=0;" edge="1" parent="1" source="syKNFbUEqoHMrX5vQTZi-6" target="syKNFbUEqoHMrX5vQTZi-5">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="440" y="189.5" as="sourcePoint" />
            <mxPoint x="520" y="189.5" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-15" value="" style="endArrow=classic;html=1;rounded=0;exitX=0.5;exitY=1;exitDx=0;exitDy=0;entryX=0.5;entryY=0;entryDx=0;entryDy=0;" edge="1" parent="1" source="syKNFbUEqoHMrX5vQTZi-3" target="syKNFbUEqoHMrX5vQTZi-4">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="260" y="210" as="sourcePoint" />
            <mxPoint x="340" y="210" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="syKNFbUEqoHMrX5vQTZi-16" value="" style="endArrow=classic;html=1;rounded=0;exitX=0.5;exitY=0;exitDx=0;exitDy=0;entryX=0.5;entryY=1;entryDx=0;entryDy=0;" edge="1" parent="1" source="syKNFbUEqoHMrX5vQTZi-3" target="syKNFbUEqoHMrX5vQTZi-1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="190" y="290" as="sourcePoint" />
            <mxPoint x="190" y="230" as="targetPoint" />
          </mxGeometry>
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
drawio…]()


#### (2) What can go wrong?
-Threats (using STRIDE):

 -Spoofing: Hackers pretending to be real users.
 -Tampering: Attackers modify or delete design files.
 -Repudiation: Users deny actions because of poor logging.
 -Information Disclosure: Private files get leaked.
 -Denial of Service (DoS): Servers crash due to too much traffic.
 -Elevation of Privileges: Attackers get admin-level access.

-Top Risks:

 -Stolen passwords through phishing emails.
 -Data leaks exposing customer designs.
 -Hackers crashing the website with a DoS attack.
#### (3) What are we doing about it?
-Steps to Reduce Risks:

 -Limit login attempts to block brute force attacks.
 -Require MFA for all users.
 -Encrypt all customer data (in storage and in transit).
 -Monitor for unusual behavior (e.g., logging into multiple accounts quickly).
 -Regularly test the system for security weaknesses.

-Risk Management (META):

 -Mitigate: Use encryption and strong login protections.
 -Eliminate: Remove unused features that could be attacked.
 -Transfer: Get cyber insurance for data breaches.
 -Accept: Low-risk issues like small delays in service.
#### (4) Did we do a good job?

-Test security regularly with ethical hackers (pentests).
-Update defenses based on new threats.
-Collect customer feedback to spot unnoticed problems.
-Review the system every three months for improvements.

### Sources

-Braiterman et al 2020: Threat Modeling Manifesto
 Available at: [https://www.threatmodelingmanifesto.org]

-OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet
 Available at: [https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html]

-Darknet Diaries Podcast
 Episode referenced: "The Beirut Bank Job"
 Available at: [https://darknetdiaries.com]

-Karvinen 2024: Information Security Course
 Task source: [https://terokarvinen.com/information-security/]
