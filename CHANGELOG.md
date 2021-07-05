# Changelog

## [1.0.4] - 2021-07-05

- Updated compatibility section in `README.md`
- Updated dependencies.

### Added

- Realtime Camera-based environment map to the `ZapparCamera` component.
- `Realtime Camera-based Reflections` section to `README.md`
- `CameraEnvironmentMap` tests.
- Added TypeDoc.

## [1.0.3] - 2021-05-04

### Fixed

- GitHub badge line-break in `README.md`
- Issue where camera source could not be a string.

### Changed

- Minor ESLint formatting changes in tests.

### Added

- `onFirstFrame` callback prop to `ZapparCamera` component. This gets called when the first camera frame is processed.
- `First Frame` section to `README.MD`

## [1.0.2] - 2021-04-09

- Open-sourced on GitHub.
- Updated Dependencies.
- Eslint fixes.

### Added

- Ability to use img/video elements as camera sources.
- Face and Image tracking tests.
- Exposed `LogLevel`, `setLogLevel`.
- `permissionRequest`(true) prop to `ZapparCamera`.
- `LICENCE.MD`.
- issues/repo urls to `package.json`
- Build badge to `README.md`

### Removed

- `skipVersionLog`.

### Changed

- Licencing copy in `README.MD`
- Changed licence to `MIT` in package.json

## [1.0.1] - 2021-04-01

- Cleaned up internal usage of forwardRef

### Added

- `makeDefault` prop to ZapparCamera.
- `renderPriority` prop to ZapparCamera.
- `README.MD:` Added `makeDefault` and `renderPriority` documentation to Camera section.

### Fixed

- `PlacementUI` styling.

## [1.0.0] - 2021-03-31

- Updated dependencies
- Switched to yarn

### ⚠️ Breaking

- react-three-fiber updated to 6.0.1
- You will now need to set `ZapparCamera` as your main camera using `useThree(state => state.set)`

### Fixed

- `Prettier` `printWidth` now matches `eslint` `max-len`

### Changed

- Minor refactor of all components.
- Tracker Components:
  - Removed `useUpdate` in favor of `useRef` as `@react-three/fiber` discontinued the hook.
  - Tracker Components which make use of forwardRef, now have correct ref types.

### Added

- An easy to use placement UI for Instant Trackers. (`placementUI` prop for `InstantTracker` component)
- `@react-three/drei` dependency

### Removed

- makeDefault prop from `ZapparCamera` component. This should now be handled by users.
- `README.MD`: Camera's `makeDefault` documentation.

## [0.1.27] - 2021-03-09

- Updated dependencies

### Added

- sources prop to `Camera` component, allowing custom video devices to be used.

## [0.1.26] - 2021-02-24

### Fixed

- Missing `forwardRef` parameters

## [0.1.25] - 2021-02-19

### Changed

- `README.MD`
  - Temporally removed preview gif

## [0.1.24] - 2021-02-19

### Changed

- `README.MD`
  - Tidied up code snippets
  - Added `create-react-app` instructions
  - Added `snapshot` guide to `Camera` section
  - Added preview gif

### Fixed

- Issue where `<Loader>` component would not dispose of itself.

### Added

- React router test
- `skipVersionLog` for silencing version logs

### Fixed

- `<Loader>` now honours `style` and `onLoad` changes (added to `useEffect`'s dependency list)

## [0.1.22] - 2021-02-08

### Added

- `Pipeline` object to be used when removing and adding canvas (`react-router-dom` support)
- `react-router-dom` section to README.MD
- `pipeline?` prop to `ZapparCamera`,  `InstantTracker`, `ImageTracker`, `FaceTracker` components.
- `model?` prop to `FaceTracker` component

### Fixed

- Tracker's callbacks are now cleaned up when dismounted

## [0.1.20] - 2020-12-08

### Added

- Exposed `Types` interface containing types for primitive three tracker objects.

### Fixed

- `ZapparCamera` component now correctly supports `poseMode="anchor-origin`

## [0.1.6-0.1.19] - 2020-12-08

### Added

- Keywords to `package.json`
- `zapparCanvas` id to `ZapparCanvas` component
- `create-react-app` templates will follow versioning of this package.

## [0.1.5] - 2020-12-11

### Changed

- Updated dependencies.
- `README.md` removed some incorrect info.

### Added

- Keywords to `package.json`

## [0.1.4] - 2020-12-03

### Changed

- Camera prop is now optional when constructing trackers.
- Tidied up internal interfaces.
- `README.md` updated to reflect this patch.

## [0.1.3] - 2020-12-02

### Added

- `animations` props to tracker components (needed for three 0.123.0)

### Changed

- React Three Fiber peer dependency to ">= 5.2.1"

## [0.1.2] - 2020-12-01

### Added

- `npx create-react-app` instructions to README.md

### Changed

- `README.md` bootstrap project markdown formatting.

## [0.1.1] - 2020-12-01

Initial release
