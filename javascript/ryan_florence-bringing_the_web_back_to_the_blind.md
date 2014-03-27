# Bringing the web back to the blind

Ryan Florence, @ryanflorence, Instructure

7 million visually disabled users in just Wyoming, N. Dakota, S. Dakota, Colorado, Deleware, Rhode Island, Vermont, and New Hampshire.

Making a website accessible for the blind

* Learn to use a screen reader
* Headers, landmarks, links, and form fields.

role="banner" create a banner landmark
aria-label-"..." What you want the reader to say
aria-labelled-by="..."

Accessibility navigation to move to next header of the same level. Semantics matter.

HTML5BP has .hidden, .visuallyhidden (no screen but yes screenreader)

`<div aria-hidden="true">...</div>` to hide from screen reader.

Bootstrap tabs aren't very screenreader-friendly. “So what blind people have to do is say, ‘I bet this is a Bootstrap website’ and click the link and hope it’s what they wanted.”

Progressive enhancement is doing it wrong for accessibility

* Screenreaders all execute javascript

WAI ARIA Web Accessibility Initiative Accessible Rich Internet Applications - Documents how to do it.

"When we work on making our devices accessible by the blind, I don't consider the bloody ROI." - Tim Cook, Apple CEO
