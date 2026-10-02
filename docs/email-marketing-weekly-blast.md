# Email Marketing — Weekly Email Blast

**Frequency:** Weekly
**Platform:** GoHighLevel (GHL)
**Owner:** (add name)
**Last reviewed:** (add date)

---

## 1. Trigger

Begin the weekly email marketing process by checking whether a qualifying
new listing is available for promotion.

!!! question "Decision Point"
    **Is there a qualifying new listing available?**

    - **YES** → Follow **Path A: New Listing Email Blast**
    - **NO** → Follow **Path B: Blog Email Blast**

    Only one path is completed for each weekly email blast.

---

## PATH A — New Listing Email Blast

### 2. Pull Listing Information

1. Open the property listing in MLS.
2. Pull the required property information from the MLS listing.
3. Use the MLS listing as the **source of truth** for property information.

### 3. Generate Email Content

1. Run the MLS listing details through AI.
2. Generate the property highlights and email draft.
3. Proofread the AI-generated email.
4. Compare the email against the MLS listing.
5. Correct any information that does not match the property.

### 4. Build Email in GHL

1. Open the GHL Email Builder.
2. Add the approved email copy.
3. Download the required property photos from OneDrive.
4. Upload the photos to GHL Media Storage.
5. Add the photos to the email.
6. Add the required property information and links.
7. Review the completed email.

### 5. Configure Tracking

Add the required action-based tracking tags:

| Tag | Trigger / Action |
|---|---|
| `marketing email` | Contact opened email |
| `email` | Contact unsubscribed |
| `hardbounced` | Email hard bounced |
| `softbounced` | Email soft bounced |
| `click marketing` | Link clicked |
| `fb` | Facebook link clicked |
| `ig` | Instagram link clicked |
| `linkedin` | LinkedIn link clicked |

### 6. Configure Batch Sending

| Setting | Value |
|---|---|
| Receiver Tag | `Buyers` |
| Batch Quantity | 300 contacts |
| Batch Interval | 15 minutes |
| Sender Name | (add required sender name) |
| Sender Email | (add required sender email) |
| Schedule Date | (add scheduled date) |
| Schedule Time | (add scheduled time) |

### 7. Dimitrios Review

1. Send the email draft to Dimitrios for review.
2. Review his requested changes.
3. Update the email as needed.
4. Repeat revisions if necessary.
5. Once the final email is approved, proceed with the batch email.

### 8. Send & Monitor

1. Process the approved batch email for sending.
2. Check email statistics periodically.
3. Monitor:
    - Send/delivery quality
    - Opens
    - Link interactions
    - Unsubscribes
    - Hard bounces
    - Soft bounces
4. Monitor the campaign until sending is complete.
5. Confirm the campaign finishes without errors or unusually high bounce activity.

---

## PATH B — Blog Email Blast

> Use this path **only** when there is no qualifying new listing available for the weekly email blast.

### 2. Select Social Post

1. Select one existing social media post to use for the weekly email marketing content.
2. Determine the intended audience for the content:
    - Buyer
    - Seller
    - Other applicable audience

### 3. Build & Publish Blog Post

1. Build a blog post based on the selected social media content.
2. Develop the blog around the content's intent and target audience.
3. Add an appropriate CTA based on the blog's intent.
4. Review the completed blog post.
5. Publish the blog post.
6. Confirm the published blog post is accessible.

### 4. Generate Email Content

1. Run the completed blog post through AI.
2. Generate the email blast draft.
3. Proofread the email.
4. Confirm the email matches the blog post's intent and content.
5. Correct any inaccurate or unsupported information.

### 5. Build Email in GHL

1. Open the GHL Email Builder.
2. Add the approved email copy.
3. Add CTA buttons directing recipients to the blog post.
4. Create a video-style thumbnail with a play button.
5. Link the thumbnail to the blog post.
6. Review the completed email and links.

### 6. Configure Tracking

Add the required action-based tracking tags:

| Tag | Trigger / Action |
|---|---|
| `marketing email` | Contact opened email |
| `email` | Contact unsubscribed |
| `hardbounced` | Email hard bounced |
| `softbounced` | Email soft bounced |
| `click marketing` | Blog Post link clicked |
| `fb` | Facebook link clicked |
| `ig` | Instagram link clicked |
| `linkedin` | LinkedIn link clicked |
| `website` | Website link clicked |

### 7. Configure Batch Sending

| Setting | Value |
|---|---|
| Receiver Tag | `Buyers` |
| Batch Quantity | 300 contacts |
| Batch Interval | 15 minutes |
| Sender Name | (add required sender name) |
| Sender Email | (add required sender email) |
| Schedule Date | (add scheduled date) |
| Schedule Time | (add scheduled time) |

### 8. Dimitrios Review

1. Send the email draft to Dimitrios for review.
2. Review his requested changes.
3. Update the email as needed.
4. Once the final email is approved, proceed with the batch email.

### 9. Send & Monitor

1. Process the approved batch email for sending.
2. Check email statistics periodically.
3. Monitor: delivery quality, opens, link interactions, unsubscribes, hard bounces, soft bounces.
4. Monitor the campaign until sending is complete.
5. Confirm the campaign finishes without errors or unusually high bounce activity.

---

## Weekly Decision Flow

```mermaid
flowchart TD
    A[Weekly Email Marketing Trigger] --> B[Check for qualifying new listing]
    B --> C{New listing available?}
    C -->|YES| D[PATH A: New Listing Email Blast]
    C -->|NO| E[PATH B: Blog Email Blast]

    D --> D1[MLS] --> D2[AI Draft] --> D3[Proofread] --> D4[GHL Email] --> D5[Photos] --> D6[Tracking] --> D7[Batch Setup] --> D8[Dimitrios Review] --> D9[Approval] --> D10[Send] --> D11[Monitor]

    E --> E1[Select Social Post] --> E2[Build Blog + CTA] --> E3[Publish] --> E4[AI Email Draft] --> E5[Proofread] --> E6[GHL Email] --> E7[CTA / Thumbnail] --> E8[Tracking] --> E9[Batch Setup] --> E10[Dimitrios Review] --> E11[Approval] --> E12[Send] --> E13[Monitor]
