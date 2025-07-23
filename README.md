# Professor-Messer-CompTIA-Security-SY0-701-Study-Notes
A comprehensive appendix of study notes, From **Professor Messer's** free YouTube course "**CompTIA SY0-701 Security+ Training Course**"

The **CompTIA Security+** certification is a widely recognized and valued credential in the cybersecurity industry. It is often considered by companies when evaluating candidates for entry-level and intermediate security roles.

This repository is not intended to explain the exam itself in great detail. Anyone using these notes to study is encouraged to review the official exam objectives and understand the core topics outlined by CompTIA before pursuing certification.

The primary purpose of this repository is to share knowledge by providing clear, structured notes based on the **Security+ course by Professor Messer** in an accessible, **text-based format**.

Most of the study notes in this repository are based on the **free Security+ course by Professor Messer**, available on **YouTube**. These courses are widely respected for their **comprehensive coverage and in-depth explanations**, making them a valuable resource for anyone preparing for the certification.

Notes are organized using dropdown menus, with each section corresponding to one of the official Security+ exam objective domains. You can download the full list of objectives and other official resources from the CompTIA website:

Link: https://www.comptia.org/en-us/certifications/security/

## Exam Objective Domains
<details>
  <summary><strong>1.0 General Security Concepts</strong></summary>
<details>
  <summary><strong> 1.1 Security controls</strong></summary>

## Good security measures aim to do these 3 things.

- **1 Prevent security events.**

- **2 Minimize the impact.**

- **3 limit the damage.**


## Control Catergories

## Technical Controls
- these are Controls that are implemented using **systems**.

## Managerial Controls
- Administrative controls assoicated with security design and implementation.

- **Security policies**, Are part of standard operating procedures for managerial controls.

## Operational controls
- These types of controls are implemented by people rather than systems. Examples include Security Guards, or a Phishing Awareness program.

## Physical Controls
Physical controls aim to limit physical access securely, Examples include.
- 1 Guard shack.
- 2 Lock.
- 3 Fences.
- 4 Badge Readers.

## Control Types.
There are also control **'types'** That go along with **control catergories**. There are **6** Control types we will study.

- 1 Preventive.

- 2 Deterrent.

- 3 Detective.

- 4 Corrective.

- 5 Compensating.

- 6 Directive.

## Preventive
Blocking access to a resource.
The preventive control type prevents access to anything we don't want accessed, At least not by the wrong people. Examples include:
- **Firewall rules.**
- **Following security policy.**
- **A guard that checks ID cards before allowing access into a building or area.**
- **Enabling door locks.**

**TIP:** A good exercise is to try and understand where a **control type** fits into a **control catergory** For example.
A **firewall** is a **preventive control type** And since it is utilized through a digital system it falls in the **control catergory of "Technical"**

# Deterrent
- The goal of the **detterent security control type** is to make an attacker think twice before attempting to intrude, This does not directly prevent access, But is the more outward security measure, Examples Include: Posted warning signs. 

# Detective
**Detective control types can Identify and Log and intrusion attempt, This control type may not prevent access, But does notify us of potential problems that need further investigation. Examples include:** 
1 Collecting and reviewing system logs.
2 Review login Reports.
3 Perform regular patrol of a property.

# Corrective 
**This control type is applied AFTER an event has been detected, For example if you have gotten a **(True Positive)** Result from a detective control type, Now you have to correct the problem/event. Examples Include:**
1 Restoring from backups leading to mitigation of a ransomware infection.
2 Contacting law enforcemnet to manage criminal activity.
3 Using a fire extinguisher.

# Compensating 
**This control type is used when the existing controls are not sufficient to deal with the event at hand, Most of the time this type of control is temporary, For example, If a business has an application, And they've been told that there is a dangerous vulnerability in the code, That business may need to employ some form of compensating control, Implementing some other rules while waiting for a patch to their application. In order to continue business operations.**

# Directive
**This control type directs a subject towards security compliance, For example employees may be asked to store all sensitive files in an encrypted/secured folder.**
**Note:** This is a realitively weak security control.

## ENDING NOTES

- There are many catergories of control
- Some organizations will combine types
- New security controls are created as systems and processes evolve
- Some organizations may use vastly different controls
</details>

<details>
<summary><strong> 1.2 the CIA triad </strong></summary>
  
# The CIA Triad, A combination of principles.

> May sometimes be refered to as the **"AIC"** Triad, In efforts to not confuse the acronym with the **"Central Intelligence Agency"**

## The "C" - Confidentiality

Aims to prevent disclosure of information to anyone who is unauthorized, Whether that be an individual or system.

Certain information should only be accessed by certain people, There are a few good ways to implement confidentiality.

**1** Encryption : Encoding messages so only certain people can read them.

**2** Access controls : Selectively restrict access to a resource, We see this example a lot in cybersecurity and that's because it works, An example is someone working in the shipping department of an organization, Under no circumstances should they have any access to the machines or information related to the accounting department of that same organization, And vice versa, You may also hear the term **"Least Priviledge"** Which means a person/(Employee) is only given as much resources and information as it takes to complete their task.

**3** Two-Factor Authentication : Additonal confirmation before information is disclosed.

## The "I" - Integrity
No one principle is better then the next in the CIA triad, But integrity is extremely important, It's the proccess of verifying information, When any type of data is sent over the internet, It comes in contact with a bunch of different devices that we never see, The goal of integrity is to make sure that information does not change one bit through that proccess, Examples include hashing, (A fixed length of mapped data that can prove integrity.) Digital Signatures, Certficates (Usually combined with a digital certficate to verify an entity)

## The "A" - Availability
information is always accessible to the authorized users. Examples of **maintaining availability** include,
> Building services that will always be available.
> Fault Tolerance (System will continue to run even when failure occures)
> Patching.

## END

</details>

<details>
<summary><strong>1.2 Non-Repudiation</strong></summary>

## nonrepudiation

**1. "Assurance that a contract cannot later be denied by either of the parties involved."**
**2. "Assurance that the claimed sender or recipient is in fact the party who sent or received a given message."**

## Proof Of Integrity 
> Verify data doe's NOT CHANGE.
In cryptography for example, Proof of integrity can be accomplished by using a **hash**, This can be thought of almost as **'Digital Fingerprint'** For data.
> If the data changes the hash changes.
> For example all of the data that makes up a singular program would be given a unique hash, So when we download that program we can check the hash to make sure we are getting the intended download, Nothing is missing, And it's exactly what we expect!

## Hashing example -SHA256

> Here's a simple example of how hashed data changes based on simple inputs

> Safe! --> SHA256 --> 622882d3f539ad4cf271f6e336403983ed31a67d6be418d50d2d05aa8088c3d2 <-- Our hashed value of the input.

> Safe --> SHA256 -->  4f9f0dabcd26ae53ecb47f632b5fc4d82f35d4110e2b0fb1a3bad7fce0c5a898 <-- Our hashed value of the input.

> Notice the small difference in the input, That changes the entire hash!

We covered how to prove that we are working with the correct data, And we know if data has been changed, But how do we prove the source or Sender, Of the data ?

## Proof Of Origin
This practice can go by a few names/terms, But we'll just stick to authenticaiton, A popular way of doing this is through **digital signatures** It's the process of using asymetric encryption (Public & Private Keys) You can read more about this here. 

> https://en.wikipedia.org/wiki/Digital_signature

## END STUDY


</details>



<details>
  <summary><strong>2.0 Threats, Vulnerabilities, and Mitigations</strong></summary>

</details>

<details>
  <summary><strong>3.0 Security Architecture</strong></summary>

</details>

<details>
  <summary><strong>4.0 Security Operations</strong></summary>

</details>

<details>
  <summary><strong>5.0 Security Program Management and Oversight</strong></summary>

</details>
