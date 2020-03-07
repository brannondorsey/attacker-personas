# Threat Classes & Attacker Personas

> "Know your enemy" - Sun Tzu, The Art of War

Modern cybersecurity practices use threat modeling to identify weak components in a software system, and use that information to design and prioritize defenses against intrusion and attack. Threat modeling ask questions like "what are the weakest parts of our system", "how could an attacker breach our network", and "what types of attacks should we be worried about." To better answer these questions, it is useful to understand the types of attackers you or your organization may fall victim to.

Fields like User Experience design, Advertising, and Marketing have long used contrived personas to better understand their users and customers. These techniques are easily transferable to the security industry and can be used to create attacker personas. By identifying several common classes of attackers, you can use them to improve your threat model. Different types of attackers have different means, motives, and resources and their attacks leave different signatures. Knowing your enemy goes a long way in defending against them.

I've compiled a short list of eight attacker personas to help you get started below. This list is by no means exhaustive, but all of these classes exist in some capacity today, and are real and present danger to many systems in the wild.

## The Nation State

*Advanced Persistent Threat (APT) | Limitless Budgets*

Nation state attackers are well funded, coordinated, state-sponsored, and militant in execution. Their motivations are strategic and can include stealing trade secrets and theft or destruction of property or data. Nation state attackers often present themselves as Advanced Persistent Threats (APTs): they are highly skilled and their attacks are calculated and narrowly targeted. Full compromise of an APT's target is nearly inevitable. Once they have a foothold, it's not uncommon for the threat actors to remain silently present in a system or network for months or years before exfiltrating data or damaging systems. Historically, these threats have originated from China, Russia, North Korea, Israel, and the United States.

## The Script Kiddie

*Skill-limited | Borrows Offensive Scripts and Toolkits | Resourceful | Careless*

The script kiddie is an unskilled hacker who reuses scripts and leverages automated attack tools to compromise a victim's system. What they lack in technical skill they make up for in resourcefulness. Their attacks are often broadly scoped and noisy, but quite effective if they are not detected and automatically protected against. Unpatched or outdated software exploits are a common attack vector for script kiddies, as they can re-use existing PoC code and tools like metasploit to scan and target systems that don't receive regular package updates. The power of the script kiddie increases each year as the number of advanced attack scripts and automated tooling is released on the public internet.

## The Security Researcher

*Bug Bounty Hunter | Academic Researcher | Independent Researcher*

The security researcher is a white- or gray-hat hacker looking to find undisclosed or original vulnerabilities in software systems. They are highly skilled and perhaps more importantly, knowledgeable about a wide range of attack methodologies and techniques. They often communicate with security teams and use coordinated disclosure and CVEs to announce and remediate the vulnerabilities they find. They are economically or socially motivated to discover vulnerabilities, and while they often are well-intended, their behavior can have unintended consequences for their attack targets which can lead to information leak, DoS, and bad press.

## The Fraudster

*Spammer | Malvertiser | Card Fraudster | Ransomware*

The fraudster's primary goal is monetary, and their techniques range from email spamming to illicit cryptocurrency mining and ransomware. Fraudsters often live in countries that condone their behavior or don't have extradition laws with the US, and therefore aren't particularly worried about being caught.

## The Compromised Employee

*Rogue Employees | Employees with Compromised Devices | Ex-Employees*

The compromised employee can leverage insider knowledge and access to exert catastrophic damage to an organization. The risk of compromised employees extends far beyond rouge or ex-employees, as one of the most common attack vectors today is through compromised employee devices or client-side attacks. Without proper role-based access control, low-ranking employees can be as dangerous as admins.

## The Hacktivist
*Political | Hacking Group | Collaborative | Leakers*

Hacktivists are politically motivated. They often organize in groups, and attack targets that represent or support ethics they disagree with. Hacktivists are known for leaks and DDoS attacks and often leave calling cards or publicly claim responsibility for their attacks.

## The Unlucky

*Edge Cases | End-of-life Software | Confused Users*

The unlucky or confused user isn't intending to compromise a system, but their behavior or negligence could inadvertently lead to a security incident. Unlucky users are inadvertent masters of misuse: They are confused by UIs, they repeatedly execute actions without understanding their meaning or consequence, and they are likely to be using out of date web browsers or operating systems. If a minor bug exists in production, these users will find a way to trigger it. If that minor bug turns out to be a major bug, your team may have a crisis on their hands.

## The Package Poisoner

*Trusted Third Party | Open Source Maintainer | Browser Extension Purchaser*

The package poisoner authors or gains control of a popular software package or dependency and uses it as malware. Long dependency chains and user trust can be easily subverted by a seemingly well-intended open source maintainer, or new owner of a much-loved program or addon. Now more than ever developers are relying on shared modules, dependencies, front-end themes, and browser extensions, all written and maintained by third parties. The package poisoner knowingly subverts a user's or developer's trust to execute arbitrary code on privileged machines and devices.
