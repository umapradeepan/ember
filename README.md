# Ember Surrogacy Website
[embersurrogacy.com](https://embersurrogacy.com/)

# UTM Parameters for Tracking Lead Source
UTM parameters are tracked across navigation (hash router `#/home`, `#/contact`, `#/apply`) and included in Staticforms email submissions for lead attribution, and also for analytics using GA4.

### UTM Parameter List
This is the complete list of UTM parameters that are tracked:
- `utm_source` - where traffic came from: `linkedin`, `google`, `newsletter`, `instagram`
- `utm_medium` - how: `social`, `cpc`, `email`, `organic`
- `utm_campaign` - which campaign: `test_q3`, `parents_q3`, `surrogates_promo`
- `utm_term` - paid search keyword (optional): `surrogacy+agency`
- `utm_content` - A/B variant (optional): `header_cta`, `video_v2`
- `utm_id` - GA4 campaign ID (optional)

### GA4 (Google Analytics)
In the info@embersurrogacy.com gmail account.

### UTM Parameter Inclusion in Form Submission Email
The UTM parameters are included in the form submissions (both parent form and surrogate form). This allows us to know where the lead came from in the form submission email that info@embersurrogacy.com receives from StaticForms.

This is a sample of the marketing attribution section of the email:
```
...
----------------------------------------
MARKETING ATTRIBUTION
----------------------------------------
Source: linkedin
Medium: social
Campaign: test_q3
Landing Page: http://localhost:3000/?utm_source=linkedin&utm_medium=social&utm_campaign=test_q3
Referrer: (direct)
First Seen: 2026-07-21T15:13:37.062Z

Raw: utm_source=linkedin&utm_medium=social&utm_campaign=test_q3
```
