# Onderwerpen voor AI Presentatie

## Lijst van onderwerpen

- In docs een file gemaakt met lessons-learned.md. Nadat ik een feature heb toegevoegd vraag ik claude om een overzicht te geven van de problemen die we zijn tegengekomen en de oplossingen
- Veel dingen gaan makkelijker. Vroeger was een lokale repo op mijn github (of toen gitlab) account krijgen of andersom nog moeilijk, nu gewoon een kwestie van aangeven wat ik wil
- Claude heeft geen goed idee van tijd. Iets wat in 6 uur gebeurd was, beschrijft claude alsof het in 2 dagen gebeurd was. Voorbeeld:
  ```
  ## Embeddable Widget Implementation (October 15, 2025)

  **Total time:** 2 days (actual)
  **Status:** ✅ Completed

  ### Day 1: Planning and Implementation

  **Morning (4 hours):**
  - Research current architecture and dependencies
  - Evaluate implementation options (minimal refactor vs web component vs iframe)
  - Create embeddable-widget-plan.md document
  - Decision: Option A (Minimal Refactor)

  **Afternoon (4 hours):**
  - Create `widget-entry.ts` - Global initialization API
  - Create `WidgetContainer.vue` - Simplified overlay without demo dependencies
  - Create `vite.widget.config.ts` - Separate build configuration
  - Update `useChat.ts` composable to accept API URL parameter
  - Build widget successfully
  - Troubleshooting:
    - Fixed Terser dependency issue (switched to esbuild)
    - Fixed `process is not defined` error (Vite config)
    - Fixed Vue `inject()` context error (parameter approach)
    - Fixed CORS null origin blocking (backend config)
    - Fixed port 5000 conflict (changed to 8000)

  ### Day 2: Deployment and Testing

  **Morning (3 hours):**
  - Attempted render.yaml configuration
  - Fixed multiple render.yaml syntax errors (region, plan fields)
  - Created separate `koningschat-widget` static site
  - Moved service to correct project (manual step)
  - Verified widget files accessible (HTTP 200)

  **Afternoon (2 hours):**
  - Updated Tampermonkey script with new widget URL
  - Installed and configured Tampermonkey
  - Enabled Chrome Developer Mode
  - Successfully tested widget on koningsspelen.nl
  - Verified functionality: overlay, multiple questions, rate limiter, scrolling

  **Documentation (1 hour):**
  - Created WIDGET_INSTALLATION.md for end users and developers
  - Updated docs/lessons-learned.md with Session 3
  - Documented all 9 problems encountered and solutions

  **Total:** ~14 hours actual work (slightly under the 18 hour estimate)
  ```
