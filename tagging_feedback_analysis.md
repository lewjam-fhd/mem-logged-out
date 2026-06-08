# Tagging Feedback Analysis - Usabilla Audit
**Date:** June 4, 2026  
**Source:** Slack Channel C09NBPMCVK2  
**Total Feedback Items:** 8

---

## Executive Summary

Analysis of 8 usabilla feedback items related to tagging reveals significant usability issues, particularly around:
- **Critical UI bugs** (tagging tools disappearing across browsers)
- **Workflow inefficiencies** (excessive clicks for common operations)
- **Technical limitations** (PID recognition failures, wrong name associations)
- **Feature gaps** (bulk operations, permissions on others' memories)

---

## All Tagging-Related Feedback

### 1. **Unable to Tag in Memory - Technical Error**
- **Mood:** 2/5 😟
- **NPS:** 9/10
- **Issue:** "unable to tag her in a memory. It says 'try again later.'"
- **Context:** User also dealing with duplicate profiles (LN1J-SC8 and G5MW-PQN)
- **Platform:** Windows 10, Chrome 148
- **URL:** https://www.familysearch.org/en/memories/gallery/

### 2. **PID Recognition Failure**
- **Mood:** 3/5 😐
- **NPS:** 9/10
- **Issue:** "I copy the profile number, paste it into the Tag search box, and the person isn't recognised so I only get Add with no link to the profile"
- **Details:** 
  - Inconsistent problem - some PIDs work (wife Hendrina, daughter Gertrude), others don't (Heinrich G9YQ-575, other daughters)
  - Also requests ability to link to specific parts of PDF documents (not just images)
- **Platform:** Windows 10, Chrome 146
- **URL:** https://www.familysearch.org/en/tree/person/memories/LRFK-63T

### 3. **Partial Tag Deletion Workflow Pain** ⭐ HIGH IMPACT
- **Mood:** 4/5 😊
- **NPS:** 10/10
- **Issue:** When memory uploaded directly to person's page, tag is incomplete and requires "improve tag" before deletion
- **User Story:** "I just helped a public guest through the process of deleting over 160 partial tags on a single person's page. It took a lot of clicks."
- **Current Workflow:** Open memory → gear icon → improve tag → green checkmark → delete → confirm delete → back arrow (7 steps per tag!)
- **Suggestions:**
  - Add "delete tag" option directly on edit tag menu
  - Allow multi-select to remove tags from multiple memories at once
- **User:** Elder Kevin Augustus Long, Support Center service missionary
- **Platform:** Windows 10, Chrome 148
- **URL:** https://www.familysearch.org/en/memories/gallery/my-archive

### 4. **Critical UI Bug: Tagging Tools Disappeared** 🚨 CRITICAL
- **Mood:** 1/5 😠
- **NPS:** 0/10
- **Issue:** Editing tools disappeared from right side of tagging page
- **Progression:** Tools disappeared first in Chrome, then Edge, then Firefox
- **Impact:** "Memories has become un-usable!"
- **User Need:** Changing photos from Private to Public, viewing existing tags
- **User:** Bill Buchanan (genealogistbuchanan@gmail.com)
- **Platform:** Windows 10, Chrome 147
- **URL:** https://www.familysearch.org/en/memories/gallery
- **Note:** User mentions previous feedback was ignored

### 5. **Permission Limitation on Others' Memories**
- **Mood:** 3/5 😐
- **NPS:** 7/10
- **Issue:** "Please give us the ability to add tags and titles to memories uploaded by others, such as deceased family members"
- **Platform:** Windows 10, Chrome 147
- **URL:** https://www.familysearch.org/en/tree/person/memories/KJW7-RQ5

### 6. **Browser Compatibility Issue**
- **Mood:** 2/5 😟
- **NPS:** 6/10
- **Issue:** "It is a total pain that I have to switch to Firefox in order to do tagging now!!!!"
- **Platform:** Windows 10, Chrome 147
- **URL:** https://www.familysearch.org/en/tree/person/memories/L67Z-TMM

### 7. **Tag Sizing Workflow Inefficiency**
- **Mood:** 2/5 😟
- **NPS:** 9/10
- **Issue:** "Once I have selected a size for the tag in a photo, can you make that the default for tag size for the other tags in that photo?"
- **Use Case:** Group photos (not individual portraits) - need to resize tag for every person
- **User:** Bill Buchanan (GenealogistBuchanan@gmail.com)
- **Platform:** Windows 10, Chrome 147
- **URL:** https://www.familysearch.org/en/memories/gallery/

### 8. **Wrong Name Association Bug**
- **Mood:** 3/5 😐
- **NPS:** 10/10
- **Issue:** "I tag my son Tyler and it labels it Tanner (my other son)"
- **Scope:** Happening on multiple accounts (user and husband)
- **Status:** User called support, couldn't resolve, directed to feedback
- **User:** shelliepayne@gmail.com
- **Platform:** Windows 10, Chrome 147
- **URL:** https://www.familysearch.org/en/memories/gallery/

---

## Main Themes

### 1. **Workflow Efficiency** (3 feedback items)
Users are frustrated by repetitive, click-heavy processes:
- Partial tag deletion requires 7 steps per tag (160 tags = 1,120 clicks!)
- Tag sizing must be reset for every person in group photos
- No bulk operations available

### 2. **Technical Reliability** (4 feedback items)
Core functionality is failing:
- PID recognition is inconsistent (sometimes works, sometimes doesn't)
- Tags associate with wrong person names
- Generic "try again later" errors with no clear cause
- Critical UI elements disappearing across multiple browsers

### 3. **Browser Compatibility** (2 feedback items)
- Chrome appears to have major issues with tagging tools
- Users forced to switch browsers to continue work

### 4. **Permissions & Collaboration** (1 feedback item)
- Users can't contribute tags/titles to memories uploaded by deceased family members

---

## Pain Points (Prioritized)

### 🚨 **Critical - Service Unusable**
1. **Tagging tools disappearing across browsers** (Feedback #4, #6)
   - Makes memories "un-usable"
   - User with NPS 0/10
   - Affects Chrome, Edge, Firefox
   - Blocker for basic operations (changing privacy settings, viewing existing tags)

### 🔴 **High Impact - Significant User Friction**
2. **Partial tag deletion workflow** (Feedback #3)
   - 7 clicks per tag
   - Real example: 160 tags = over 1,000 clicks
   - Affects support missionaries helping public guests
   - High NPS user (10/10) despite frustration

3. **PID recognition failures** (Feedback #2)
   - Inconsistent behavior creates confusion
   - Users don't know if they're doing something wrong or if system is broken
   - Blocks ability to properly link family members

4. **Wrong name associations** (Feedback #8)
   - Data integrity issue
   - User tried support, couldn't be resolved
   - Affects multiple accounts

### 🟡 **Medium Impact - Quality of Life**
5. **Tag sizing doesn't persist** (Feedback #7)
   - Repetitive resizing in group photos
   - High NPS user (9/10) willing to provide feedback

6. **Can't tag in others' memories** (Feedback #5)
   - Limits collaborative genealogy work
   - Especially impacts deceased users' contributions

7. **Generic error messages** (Feedback #1)
   - "Try again later" doesn't help user diagnose or fix issue

---

## Opportunities

### 🎯 **Quick Wins**
1. **Add direct "Delete Tag" option**
   - Remove "improve tag" step requirement for partial tags
   - Reduces clicks from 7 to ~3-4 per tag

2. **Remember tag size within photo session**
   - Default new tags to last-used size
   - Significantly speeds up group photo tagging

3. **Improve error messages**
   - Replace "try again later" with actionable guidance
   - Provide specific reasons for PID recognition failures

### 🏗️ **Medium-Lift Improvements**
4. **Bulk tag operations**
   - Multi-select memories for batch tag deletion
   - Mass privacy setting changes
   - Would dramatically reduce click counts

5. **PID recognition robustness**
   - Investigate why some PIDs work and others don't
   - Add fallback search mechanisms
   - Provide clear feedback when PID can't be found

6. **Browser compatibility fixes** 🚨
   - Debug why Chrome/Edge lose tagging tools
   - Ensure cross-browser testing in CI/CD
   - Potentially highest ROI given current broken state

### 🚀 **Strategic Features**
7. **Collaborative tagging permissions**
   - Allow family members to add tags/titles to deceased users' memories
   - Could include approval workflow for sensitive cases

8. **PDF tagging enhancements**
   - Enable linking to specific sections of PDF documents
   - Bring PDF tagging closer to parity with image tagging

9. **Smart name suggestions**
   - Fix wrong name association bug
   - Consider ML-based face recognition for tag suggestions
   - Auto-complete improvements

### 📊 **Process Improvements**
10. **Feedback loop**
    - User #4 (Bill Buchanan) mentions "previous feedback seems to have been ignored"
    - Consider more visible acknowledgment of submitted feedback
    - Communicate when reported issues are being worked on

---

## Notable User Insights

### Power Users Are Frustrated
- Bill Buchanan appears twice in feedback (genealogistbuchanan@gmail.com / GenealogistBuchanan@gmail.com)
- Elder Kevin Augustus Long is a Support Center service missionary helping public guests
- These are engaged, high-NPS users providing detailed, constructive feedback
- When power users say the system is "un-usable," that's a critical signal

### High NPS Despite Issues
- 5 out of 8 feedback items have NPS ≥ 9/10
- Users WANT to love the product but are blocked by friction
- This suggests high ROI for fixing these issues - user loyalty is there

### Cross-Account Issues
- Wrong name association happening on multiple accounts (user + husband)
- Suggests systematic data or caching issue, not user error

---

## Recommended Next Steps

1. **Immediate:** Fix disappearing tagging tools in Chrome/Edge (Feedbacks #4, #6)
2. **Short-term:** Implement direct tag deletion (Feedback #3)
3. **Short-term:** Fix wrong name association bug (Feedback #8)
4. **Medium-term:** Add tag size persistence (Feedback #7)
5. **Medium-term:** Investigate and fix PID recognition (Feedback #2)
6. **Research:** Interview power users (Bill Buchanan, Elder Long) for deeper workflow insights
7. **Long-term:** Design bulk operations for tagging
8. **Long-term:** Collaborative permissions for deceased users' memories

---

## Data Summary
- **Total feedback items:** 8
- **Average Mood:** 2.5/5 (below neutral)
- **Average NPS:** 7.8/10 (high engagement despite frustration)
- **Most common platform:** Windows 10 (8/8)
- **Most common browser:** Chrome 147-148 (7/8)
- **Critical issues:** 2
- **High impact issues:** 3
- **Medium impact issues:** 2