# Config

SaasAble uses a single source of truth for default configurations, allowing users to manage settings effectively and making it scalable for new configurations. You can configure options such as font, border, theme, locale, and more in `src/config.ts`.

{% tabs %}
{% tab title="src/config.ts" %}
```typescript
// @next
import { Archivo, Figtree, Roboto, Urbanist, Space_Grotesk, DM_Sans, Plus_Jakarta_Sans } from 'next/font/google';
import localFont from 'next/font/local';

// @types
import { ConfigProps } from '@/types/config';

export enum Themes {
  THEME_CRM = 'crm',
  THEME_AI = 'ai',
  THEME_CRYPTO = 'crypto',
  THEME_HOSTING = 'hosting',
  THEME_PMS = 'pms',
  THEME_HRM = 'hrm',
  THEME_PLUGIN = 'plugin'
}

export enum ThemeMode {
  LIGHT = 'light',
  DARK = 'dark'
}

export enum ThemeDirection {
  LTR = 'ltr',
  RTL = 'rtl'
}

/***************************  CONFIG  ***************************/

const config: ConfigProps = {
  currentTheme: Themes.THEME_AI,
  mode: ThemeMode.LIGHT,
  themeDirection: ThemeDirection.LTR
};

export default config;

/***************************  THEME - FONT FAMILY  ***************************/

const fontRobot = Roboto({ subsets: ['latin'], weight: ['100', '300', '400', '500', '700', '900'] });
const fontArchivo = Archivo({ subsets: ['latin'], weight: ['400', '500', '600', '700'] });
const fontFigtree = Figtree({ subsets: ['latin'], weight: ['400', '500', '600', '700'] });

// @hosting
const fontSpaceGrotesk = Space_Grotesk({ subsets: ['latin'], weight: ['400', '500', '600', '700'] });
const fontDMSans = DM_Sans({ subsets: ['latin'], weight: ['400', '500', '600', '700'] });

// @pms
const fontPlusJakarta = Plus_Jakarta_Sans({ subsets: ['latin'], weight: ['400', '500', '600', '700'] });
const fontClashDisplay = localFont({
  src: '../public/assets/fonts/clash-display/ClashDisplay-Variable.ttf',
  variable: '--font-clash-display'
});

//HRM
const fontSatoshi = localFont({ src: '../public/assets/fonts/satoshi/Satoshi-Variable.ttf', variable: '--font-satoshi' });
const fontUncutSanaVF = localFont({ src: '../public/assets/fonts/uncut-sans/Uncut-Sans-VF.ttf', variable: '--font-uncut' });

//@plugin
const fontGeneralSans = localFont({ src: '../public/assets/fonts/general-sana/GeneralSans-Variable.ttf', variable: '--font-general-sans' });

//@crypto
const fontUrbanist = Urbanist({ subsets: ['latin'], weight: ['400', '500', '600', '700'] });

export const FONT_ROBOTO: string = fontRobot.style.fontFamily;
export const FONT_ARCHIVO: string = fontArchivo.style.fontFamily;
export const FONT_FIGTREE: string = fontFigtree.style.fontFamily;
export const FONT_SPACE_GROTESK: string = fontSpaceGrotesk.style.fontFamily;
export const FONT_DMSANS: string = fontDMSans.style.fontFamily;
export const FONT_PLUS_JAKARTA: string = fontPlusJakarta.style.fontFamily;
export const FONT_CLASH_DISPLAY: string = fontClashDisplay.style.fontFamily;
export const FONT_SATOSHI: string = fontSatoshi.style.fontFamily;
export const FONT_UNCUT_SANS_VF: string = fontUncutSanaVF.style.fontFamily;
export const FONT_GENERAL_SANS: string = fontGeneralSans.style.fontFamily;
export const FONT_URBANIST: string = fontUrbanist.style.fontFamily;
```
{% endtab %}
{% endtabs %}
