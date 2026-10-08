# TrackTruck TP1 Completion Checklist

Last reviewed: 2026-10-08

This checklist is ordered by dependency. A task is marked complete only when its repository evidence and report evidence both exist.

## 1. Repository migration and product identity

- [x] Confirm authorization to reuse the CargoExpress repositories.
- [x] Rename `tracktruck-webapp` to `tracktruck-mobile` locally and on GitHub.
- [x] Create `develop` branches for platform, mobile, and website.
- [x] Import the authorized source histories into `feature/reuse-cargoexpress-base`.
- [x] Remove inherited generated artifacts and unsafe configuration values.
- [x] Replace CargoSystems, CargoExpress, ACME.CargoExpress, and `com.cargoexpress` identifiers with TrackTruck equivalents.
- [x] Replace inherited product logos and obsolete repository links.

## 2. Platform verification

- [x] Confirm the imported IAM, User, and Registration bounded contexts and their project structure.
- [x] Build the renamed .NET solution in Release configuration.
- [x] Run unit tests: 326 passed.
- [x] Run executable integration tests: 96 passed.
- [x] Preserve the 16 Gherkin feature files as acceptance specifications and document that the imported project has no SpecFlow bindings.
- [ ] Verify OpenAPI/Swagger generation.
- [x] Remove inherited database/JWT secrets and document environment-variable configuration.
- [ ] Record real build, test, endpoint, and commit evidence.

## 3. Mobile verification

- [x] Rename the Android namespace and application ID to `com.tracktruck.app`.
- [x] Configure the API base URL without inherited production credentials.
- [x] Build the Android application with JDK 17 and Android SDK 34.
- [x] Run the debug and release unit-test tasks successfully.
- [ ] Run available instrumented tests when an emulator or device is available.
- [ ] Verify the principal authentication, fleet, trip, alert, expense, and history flows.
- [ ] Record real build, test, screen, and commit evidence.

## 4. Website verification

- [x] Replace inherited brand, team, contact, legal, and download information.
- [ ] Validate internal navigation and legal modals.
- [ ] Validate responsive layout and browser console output.
- [x] Replace or remove links to inherited deployments and APK files.
- [x] Confirm that all 24 local assets referenced by `index.html` exist.
- [x] Render and inspect the desktop hero section in Chromium; correct the clipped logo and remove the fictitious phone number.
- [ ] Record real screenshots and commit evidence.

## 5. TP1 architecture and report

- [ ] Reconcile Chapters I-III with the reused implementation.
- [ ] Complete Chapter IV: design concepts, drivers, tactics, ADD iterations, C4, UML, and database views.
- [ ] Complete Chapter V configuration-management sections.
- [ ] Define the real Sprint 1 scope from implemented user stories.
- [ ] Add Sprint Backlog 1 and Kanban evidence.
- [ ] Add development, testing, execution, OpenAPI, deployment, and collaboration evidence.
- [x] Update repository URLs from `tracktruck-webapp` to `tracktruck-mobile`.
- [ ] Update the report version history, table of contents, references, annexes, and TP1 links.

## 6. Human evidence and submission package

- [ ] Conduct three real interviews per target segment.
- [ ] Add interview screenshots, YouTube URLs, timing, duration, summaries, and statistical analysis.
- [ ] Reconcile personas and research artifacts with the real interviews.
- [ ] Record the real execution/demo video required for Sprint 1.
- [ ] Complete TP1 ABET evidence per member without inventing participation.
- [ ] Prepare the Individual Member Performance Report in DOCX and PDF.
- [ ] Export and visually verify the final report.

## 7. GitFlow closure

- [x] Push the platform, mobile, website, and report feature branches.
- [x] Open pull requests into `develop`.
- [x] Review the available gates: GitHub reports no configured CI; local platform and mobile gates pass and the website assets/desktop hero were inspected.
- [x] Merge the verified platform, mobile, and website migrations into `develop`.
- [x] Merge the report migration into `develop`.
- [ ] Confirm every remote branch and final artifact from a clean checkout.
