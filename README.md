# React Native Quick Starter

A batteries-included React Native project template built with:

- **[Expo SDK 54](https://docs.expo.dev/)** — Managed workflow
- **[Expo Router 6](https://docs.expo.dev/router/introduction/)** — File-based routing
- **[HeroUI Native](https://heroui.com/)** — Beautiful component library
- **[Uniwind](https://docs.uniwind.dev/) + [TailwindCSS 4](https://tailwindcss.com/)** — Utility-first styling with dark mode
- **[React Native Reanimated](https://docs.swmansion.com/react-native-reanimated/)** — Performant animations
- **[@gorhom/bottom-sheet](https://gorhom.github.io/react-native-bottom-sheet/)** — Bottom sheet interactions
- **TypeScript** — Full type safety

## Getting Started

```sh
# Install dependencies
pnpm install

# Start the development server
pnpm start
```

Then press `i` for iOS, `a` for Android, or `w` for Web.

## Project Structure

```
src/
├── app/                  # File-based routes (Expo Router)
│   ├── _layout.tsx       # Root layout (Providers)
│   ├── index.tsx         # Entry redirect
│   ├── [...missing].tsx  # 404 page
│   └── (tabs)/           # Tab navigation
│       ├── _layout.tsx   # Tab bar config
│       ├── index.tsx     # Home tab
│       └── explore.tsx   # Explore tab
├── utils/
│   └── cn.ts             # className utility
├── global.css            # TailwindCSS + Uniwind + HeroUI styles
└── uniwind-types.d.ts    # Uniwind theme types
```

## Included Dependencies

| Category   | Packages                                                                |
| ---------- | ----------------------------------------------------------------------- |
| Navigation | `expo-router`, `react-native-screens`, `react-native-safe-area-context` |
| UI         | `heroui-native`, `@expo/vector-icons`, `@gorhom/bottom-sheet`           |
| Styling    | `tailwindcss`, `uniwind`, `tailwind-merge`, `tailwind-variants`         |
| Animation  | `react-native-reanimated`, `react-native-gesture-handler`               |
| Storage    | `@react-native-async-storage/async-storage`, `expo-secure-store`        |
| Utilities  | `expo-clipboard`, `expo-linear-gradient`, `react-native-svg`            |

## Deploy

Deploy on all platforms with Expo Application Services (EAS).

- **Web**: `npx eas-cli deploy` — [Learn more](https://docs.expo.dev/eas/hosting/get-started/)
- **iOS / Android**: `npx eas-cli build` — [Learn more](https://expo.dev/eas)
