# Navbar7

`Navbar7` is a responsive navigation bar component using MUI's `AppBar`, `Toolbar`, and `Box`, designed to display customizable content through the `children` prop, with dynamic styling and padding adjustments based on screen size.

{% hint style="info" %}
All available props for the Navbar7 component are defined and handled within **Component usage path** file. This allows for easy modifications to the content of the Navbar section.
{% endhint %}

**Component path**: `src/blocks/navbar/Navbar7.tsx`

**Component usage path:**  `src/app/blocks/navbar/navbar7/page.tsx`

**Preview link:** [**https://www.saasable.io/blocks/navbar/navbar7**](https://www.saasable.io/blocks/navbar/navbar7)

## Props Details

| Prop         | Type           | Description                                                                                                                                                                                                                     | Display as                                                |
| ------------ | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| **children** | `ReactElement` | A single React element or component that will be rendered inside the `StyledToolbar` of the `AppBar`. This prop allows for custom content such as logos, navigation links, or any other elements to be displayed in the navbar. | Elements that will be displayed inside the navigation bar |
