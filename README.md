# kidssafe-template

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A template for creating and sharing a community safety map. This project allows you to manage map data using simple CSV files, which can be edited in tools like Excel or Numbers. It is built upon the [KidsSafe project by Code for FUKUI](https://github.com/code4fukui/kidssafe/).

## Demo

https://code4fukui.github.io/kidssafe-template/

## Features

- Create and share a community safety map via GitHub Pages.
- Manage map points using simple CSV files, editable in Excel or Numbers.
- Easily add new data layers and custom icons by editing [index.csv](index.csv).
- Uses [Geo3x3](https://github.com/jigjp/geo3x3) for location encoding, with a simple [lookup tool](https://fukuno.jig.jp/app/map/latlng/#%E8%B6%8A%E5%89%8D%E5%B8%82).

## Getting Started

1.  **Create your repository:** Click the "Use this template" button to create a new repository.
2.  **Enable GitHub Pages:** In your new repository's "Settings", go to the "Pages" section. Select the `main` branch as the source and save. Your map will be live at `https://<your-username>.github.io/<your-repo-name>/`.
3.  **Customize your map:** Edit the `index.html` file and change the placeholder city (`〇〇市`) and district (`〇〇地区`) names to your own.

## Updating Map Data

1.  From your repository, download a data file you wish to edit (e.g., [aed.csv](aed.csv)).
2.  Open and modify the file in Excel, Numbers, or any spreadsheet application.
3.  To add new locations, use the [Latitude Longitude Map](https://fukuno.jig.jp/app/map/latlng/#%E8%B6%8A%E5%89%8D%E5%B8%82) to find the correct Geo3x3 code.
4.  Upload the modified CSV file back to the root directory of your repository.
5.  Your changes will be reflected on the live map after about a minute.

## Adding New Data Layers

You can add new categories of points (e.g., "Public Restrooms") to the map:

1.  Create a new CSV file for your data (e.g., `restrooms.csv`).
2.  Add a corresponding icon image (e.g., `restroom_icon.png`).
3.  Edit [index.csv](index.csv) and add a new line to register your layer: `Public Restrooms,restrooms.csv,restroom_icon.png`.
4.  Upload your new CSV file and icon image to the repository.

## License

MIT License