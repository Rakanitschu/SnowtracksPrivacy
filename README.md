# Snow Tracks – App Store website

Static HTML website for the Snow Tracks iOS/Android game. No Firebase or build process needed.

## Publish on GitHub Pages

1. Open https://github.com/Rakanitschu/SnowtracksPrivacy/settings/pages
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main**, **/(root)**, and click **Save**.
4. After GitHub publishes the site, verify all URLs:
   - Marketing: https://rakanitschu.github.io/SnowtracksPrivacy/
   - Privacy: https://rakanitschu.github.io/SnowtracksPrivacy/privacy.html
   - Support: https://rakanitschu.github.io/SnowtracksPrivacy/support.html
   - Security: https://rakanitschu.github.io/SnowtracksPrivacy/security.html

## Must update before submitting to Apple

The policy and pages contain deliberately visible placeholders. Replace:
- `[DEVELOPER LEGAL NAME]` in `privacy.html`
- `[CONTACT EMAIL]` in `privacy.html`
- `[SUPPORT EMAIL]` in `support.html`
- `[SECURITY EMAIL]` in `security.html`

Use a valid monitored email, verify disclosures against the final shipping build, and consider any additional German/EU website legal notice or impressum requirements. Avoid claiming that data collection is zero: Snow Tracks integrates Google AdMob and in-app purchases.

Finally update `src/services/platform.ts` in the separate, private `snowtracks` game repository to point to the live privacy URL and verified support email. The game has not been changed by this website repository.
