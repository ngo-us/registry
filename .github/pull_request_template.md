# Pull Request Template for `.ngo.us` Domain Registration

<!-- 
Thank you for applying to register a domain under the `.ngo.us` namespace. Please follow this template carefully to ensure a smooth review and approval process. Pull requests that do not meet the guidelines will be delayed or rejected.

Each section below contains instructions that you need to complete. Make sure to provide the required information in the relevant sections. These instructions are only visible when editing the pull request and will not appear in the final submission.
-->

## Checklist for Domain Registration Application

### 1. Zone File Edit
<!-- 
Ensure that the zone file (`db.ngo.us`) is edited according to the instructions in the README. Each domain block should be in alphabetical order by your organization’s name. Don't forget to include two comment lines with your organization's name and contact email. 
-->
- [ ] **Alphabetical Order**: Confirm your domain block is added in alphabetical order by your organization’s name.
- [ ] **Two Comment Lines**: 
  - First line: Full organization name.
  - Second line: Organizational contact email (must be different from the `.ngo.us` domain applied for).
- [ ] **Nameserver Entries**:
  - At least two NS (Nameserver) records with a TTL value of `86400`.
  - Correct format for the domain block (see README for examples).

Example:
```
; Happy Cat Foundation
; Submitted by networking team <happycat@example.org>
happycat 86400 IN NS ns1.example.com.
happycat 86400 IN NS ns2.example.com.
```

---

### 2. PR Description

#### a. **Intended Use of Domain**
<!-- 
Please provide as much detail as possible on how you intend to use the domain. This will help us understand the purpose of your application. The more detailed your explanation, the better.

- **Example**:  
  "We intend to use `happycat.ngo.us` to promote awareness and resources for stray cat care in our local community. The domain will host a website where visitors can learn about our work, make donations, and access our contact information."
-->



#### b. **Organization Online Presence URLs for Verification**
<!-- 
List the URLs where your organization’s online presence can be verified (e.g., social media profiles, website). These URLs should provide sufficient information about your organization’s mission and activities.

- **Example**:
  - Facebook: https://facebook.com/happycatfoundation
  - Twitter: https://twitter.com/happycatngo
-->



#### c. **Proof of Domain Mention**
<!-- 
Provide the specific URL or screenshot where the exact domain name (e.g., `happycat.ngo.us`) is mentioned on your social media or website. This will help us verify your ownership and intent to use the domain.

- **Example**:
  - Twitter bio: “Our upcoming website at happycat.ngo.us”
-->



---

### 3. Agreement to Terms
<!-- 
By submitting this pull request, you are agreeing to the terms outlined in our terms of service. Please sign the agreement below by filling in your name and organization. 
-->
By submitting this pull request, I agree to the following:
- My organization is a non-commercial entity that is not affiliated with any government body.
- My organization operates legally and in good faith according to the stated purpose.
- I have provided accurate and truthful information throughout this application.
- Other terms outlined in the Registry's [Terms of Service](https://nic.ngo.us/terms-of-service/).

<!--
**Sign the agreement by typing the following below:**
I, [Your Full Name], on behalf of [Your Organization Name], agree to the terms and conditions outlined above.
-->



---

### 4. Final Checklist Before Submitting

<!-- 
Ensure that all required steps are completed. This checklist helps prevent common issues that may delay the review process.
-->
- [ ] Zone file edited correctly, following format and alphabetical order.
- [ ] At least two valid nameservers with correct TTL (86400).
- [ ] Domain block includes required comments with organization name and contact email.
- [ ] Intended use of the domain clearly explained.
- [ ] URLs for verification included with the exact domain name mentioned on the public profile.
- [ ] Agreement to terms signed.

---

<!-- 
### 5. Monitor the PR

Once the pull request is submitted, you will need to monitor it for feedback and ensure that all automated checks pass. PRs with failing checks will not be processed. Keep an eye on your PR in case changes are requested.

Once your PR is approved and merged, please allow up to 48 hours for DNS changes to propagate.

Thank you for choosing `.ngo.us`!
-->