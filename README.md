# TRACE

## A simple framework for reporting and troubleshooting problems

> **When something doesn't work, TRACE the problem before trying to diagnose it.**

If you've ever tried to help someone who says:

> "Hey, this isn't working."

you have probably experienced the problem with that statement: **it tells you that there is a problem, but very little about the problem itself.**

TRACE is a simple framework for turning a vague problem report into useful information.

It is intended for anyone who needs to communicate a problem clearly or help someone else troubleshoot one:

- Entry-level engineers and technicians
- College students learning engineering or technical disciplines
- Operators and users of equipment or software
- IT and technical support
- Maintenance and service personnel
- Anyone who regularly finds themselves helping other people solve problems

You do **not** need to understand how the system works to use TRACE.

---

## The basic idea

A useful problem report answers five questions:

| | | | |
|---|---|---|---|
| **T**| **Task**  | What were you doing? | Establish the situation and context. |
| **R**| **Result**  | What actually happened? | Describe the observed result. |
| **A**| **Achieve** | What did you want or expect to happen? | Establish the intended result. |
| **C**| **Clues** | What evidence or additional observations do you have? | Capture information that may help explain or reproduce the problem. |
| **E**| **Extent** | What is the extent of your observations? What is affected, and what still works? | Establish the boundaries of what you actually know. |

The goal is **not** to produce a perfect technical diagnosis.

The goal is to give the next person enough information to begin troubleshooting intelligently.

---

# T — Task

### What were you doing?

Describe the activity or operation that was being performed when the problem occurred.

Think about:

- What were you trying to do?
- What were you operating, using, or interacting with?
- What was the relevant starting condition?
- What happened immediately before the problem?

### Example

> "I was trying to print a document from my laptop."

That's more useful than:

> "The printer doesn't work."

The first statement tells us what operation was actually being attempted.

---

# R — Result

### What actually happened?

Describe what you observed.

Try to separate **what happened** from what you think caused it.

For example:

> "I clicked Print, but nothing came out. The document stayed in the print queue."

is an observation.

> "The printer driver is broken."

is a diagnosis.

The diagnosis might eventually turn out to be correct, but the observation is more useful as a starting point.

### Ask:

> **What did the system actually do?**

---

# A — Achieve

### What did you want or expect to happen?

Explain the intended outcome.

This is an important question because people reporting a problem often skip it. They are understandably focused on **what went wrong**, while the person troubleshooting needs to understand **what should have happened**.

### Example

> "I expected the document to print and then disappear from the print queue."

Now we have a clear comparison:

**Expected:** Document prints and leaves the queue.  
**Actual:** Document remains in the queue and nothing prints.

That difference is the problem we need to investigate.

---

# C — Clues

### What evidence or additional observations do you have?

This is where you provide information that may help someone understand, reproduce, or diagnose the problem.

Useful clues can include:

- Exact error messages
- Screenshots or photographs
- Sounds
- Indicator lights
- Measurements
- Warning messages
- Logs
- What happened immediately before the failure
- What happened immediately after it
- Anything unusual
- Something you expected to happen that did **not** happen

### Example

Instead of:

> "The computer gave me some kind of network error."

provide:

> "The browser displayed `ERR_NAME_NOT_RESOLVED`."

The exact message may be much more useful than your interpretation of it.

**When practical, preserve the original evidence.**

A screenshot of an error is often more useful than trying to remember exactly what it said.

---

# E — Extent

### What is the extent of your observations?

**What is affected, and what still works?**

Extent establishes the boundaries of the problem.

This can include:

- What works
- What doesn't work
- What you have actually checked
- Whether the problem happens every time or only sometimes
- Whether the problem affects one thing or several
- Whether the problem occurs under particular conditions

The important distinction is:

> **Report what you checked or observed—not what you assume.**

### Example

Instead of:

> "The internet is down."

a better report might be:

> "The company website won't load. I checked two other websites and both work normally. I also tried the company website in another browser and got the same error. I haven't tried another computer."

That tells the troubleshooter much more about the **boundary of the problem**.

---

# A Complete TRACE Example

Suppose someone says:

> "My phone isn't charging."

That's a problem statement, but it leaves many questions unanswered.

A TRACE report might look like this:

### **T — Task**

> "I plugged my phone into its charging cable because the battery was low."

### **R — Result**

> "The phone did not show the charging symbol, and the battery percentage did not increase."

### **A — Achieve**

> "I expected the phone to begin charging normally."

### **C — Clues**

> "The screen briefly showed the charging symbol when I first plugged it in, then it disappeared. I tried a second cable and saw the same thing. There was no error message."

### **E — Extent**

> "The phone still turns on and works normally. I tried two cables with the same result. I have not yet tried a different power adapter or outlet."

Notice what the person **didn't** have to say:

> "I think the charging port is damaged."

They don't need to know that.

They have provided enough information for someone with the appropriate knowledge to start investigating.

---

# Another Example: A Door That Won't Open

Consider:

> "The door is stuck."

Using TRACE:

**T — Task**

> "I was trying to open the front door using the key."

**R — Result**

> "The key goes into the lock but won't turn."

**A — Achieve**

> "I expected the key to turn and unlock the door."

**C — Clues**

> "The key goes in normally. I can turn it slightly in either direction, but it stops after a small amount. I don't hear anything unusual."

**E — Extent**

> "I tried the key three times with the same result. The key works normally in the other door that uses the same key. I haven't tried another key in this lock."

That report is useful even though the person knows nothing about locks.

They have not diagnosed the problem.

They have **characterized it**.

---

# Another Example: A Website Won't Open

Suppose someone reports:

> "The website isn't working."

TRACE turns that into:

**T — Task**

> "I was trying to open the website from my laptop."

**R — Result**

> "The browser displayed an error page instead of the website."

**A — Achieve**

> "I expected the website's home page to load."

**C — Clues**

> "The browser displayed `ERR_NAME_NOT_RESOLVED`. I took a screenshot of the error."

**E — Extent**

> "Two other websites load normally. I tried the same website three times and got the same error. I haven't tried another computer."

Again, the reporter does not need to know what DNS is.

They just need to report what they observed.

---

# Why TRACE Works

There are two common problems with troubleshooting conversations.

## Problem 1: The report is too vague

> "It doesn't work."

There is almost nothing to work with.

## Problem 2: The report jumps straight to a diagnosis

> "The battery is bad."

That may be correct, but it may also send the troubleshooting effort down the wrong path.

TRACE creates a middle ground:

> **Describe the problem clearly without requiring the reporter to diagnose it.**

This is especially useful when the person reporting the problem is not an expert in the system.

A driver does not need to understand how a starter circuit works to report that a car won't start.

A computer user does not need to understand DNS to report an `ERR_NAME_NOT_RESOLVED` error.

A customer does not need to understand how a product works internally to describe what it did when they used it.

A technician does not need a complete theory of failure before reporting the symptoms.

---

# Good Troubleshooting Starts With Good Observations

TRACE is deliberately built around **observations rather than assumptions**.

Compare:

> "The battery is dead."

with:

> "The vehicle won't start. The dashboard lights come on, but they become very dim when I try to start it. I hear rapid clicking."

The second report contains more useful information while making fewer assumptions.

That is the habit TRACE is intended to encourage.

---

# Five Habits That Make a TRACE Better

These are supporting principles, not additional steps in the TRACE acronym:

- **Describe, don't diagnose.** Focus on observed behavior rather than presumed cause.
- **Report what didn't happen.** Missing expected behavior can be important evidence.
- **Be specific.** Exact observations are more useful than vague summaries.
- **Report what still works.** State what you actually checked or observed rather than assuming everything else is unaffected.
- **Capture before changing.** When practical, preserve errors, screenshots, logs, measurements, and other evidence before resetting or modifying the system.

---

# TRACE Is a Communication Framework, Not a Diagnostic Procedure

TRACE does not tell you how to repair a system.

It helps answer a more fundamental question:

> **What exactly are we trying to troubleshoot?**

Sometimes a TRACE report will simply give a troubleshooter enough information to begin investigating.

Sometimes it will dramatically narrow the search space.

And sometimes, once the problem has been described precisely, the solution becomes obvious.

That is not a failure of the framework. **Clearly defining the problem is part of troubleshooting.**

---

# Quick Reference

> ## TRACE
>
> **T — Task**  
> What were you doing?
>
> **R — Result**  
> What actually happened?
>
> **A — Achieve**  
> What did you want or expect to happen?
>
> **C — Clues**  
> What evidence or additional observations do you have?
>
> **E — Extent**  
> What is the extent of your observations? What is affected, and what still works that you actually checked or observed?

## The short version

When someone says:

> **"Hey, this isn't working!"**

ask:

> **Task?**  
> **Result?**  
> **Achieve?**  
> **Clues?**  
> **Extent?**

Then start troubleshooting.
