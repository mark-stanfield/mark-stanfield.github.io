---
# _pages/resume.md
layout: default
title: Resume Submission
---

# Resume Submission

Are you a member looking for career opportunities or an employer seeking talented Latino professionals? Submit resumes or job postings here.

**Note:** This form uses `mailto:` which opens the user's default email client. For more robust handling (e.g., storing submissions, server-side processing), consider integrating with a form service compatible with GitHub Pages.

## Submit Your Resume

<form action="mailto:careers@alpfa-gothamcity.org?subject=Resume%20Submission" method="post" enctype="multipart/form-data"> <!-- TODO: Replace with actual email address -->
    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" required>

    <label for="position">Target Position (Optional):</label>
    <input type="text" id="position" name="position">

    <label for="resume">Upload Resume (PDF or DOC):</label>
    <input type="file" id="resume" name="resume" accept=".pdf,.doc,.docx" required>

    <label for="cover_letter">Upload Cover Letter (Optional, PDF or DOC):</label>
    <input type="file" id="cover_letter" name="cover_letter" accept=".pdf,.doc,.docx">

    <label for="message">Additional Message (Optional):</label>
    <textarea id="message" name="message" rows="4"></textarea>

    <button type="submit" class="btn">Submit Resume</button>
</form>
