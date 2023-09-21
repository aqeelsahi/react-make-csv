# react-make-csv

`react-make-csv` is a JavaScript/TypeScript utility for generating CSV (Comma-Separated Values) files from data arrays. It is designed to simplify the process of creating CSV files for various use cases, such as data export, report generation, and data interchange.

## Installation

You can install `react-make-csv` using npm or yarn:

`npm i react-make-csv`
or
`yarn add react-make-csv`

## Parameters
data (Array): An array of string arrays representing the data to be converted into CSV format.

fileName (String): The desired file name for the generated CSV file.


## Example
Here's an example of using react-make-csv to create and trigger a CSV file download:
```tsx
import { generateCSV } from "react-make-csv";
import React from "react";

const Component: React.FC = () => {
  const data = [
    ['Name', 'Email'],
    ['Alice', 'alice@example.com'],
    ['Bob', 'bob@example.com'],
  ];

  const downloadCSV = () => generateCSV(data, 'myfile');

  return (
    <div
      style={{ cursor: 'pointer', textDecoration: 'underline' }}
      onClick={downloadCSV}
    >
      Download
    </div>
  );
};

export default Component;
```

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing
Contributions are welcome! If you have any bug fixes, improvements, or new features to propose, please open an issue or submit a pull request.

## Issues
If you encounter any issues or have questions or suggestions, please feel free to open an issue.

## Acknowledgments
This package was inspired by the need for a simple CSV generation utility.
Special thanks to the open-source community for their valuable contributions.

Author
Aqeel Sahi
