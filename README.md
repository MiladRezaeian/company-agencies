# company-agencies

## Description

This project aims to develop a command-line interface (CLI) program that provides functionality related to managing representatives in different regions. The program allows users to perform various operations using command-line flags, such as listing representatives, retrieving detailed information about a specific representative, creating new representatives, editing representative information, and obtaining the status of representatives in a particular region.

The program supports the following flags:

- `command`: Specifies the type of operation to be performed. It can have the following values:
  - `list`: Lists all the representatives in the specified region.
  - `get`: Retrieves detailed information about a specific representative. The user needs to provide the representative's ID.
  - `create`: Creates a new representative by capturing information such as name, address, phone number, join date, and the number of employees.
  - `edit`: Allows the user to edit the information of a representative by providing the representative's ID.
  - `status`: Displays the number of representatives and the total number of employees in the specified region.

The `region` flag represents a specific region or province within the country where the representatives are located. Users can specify the desired region when executing the program.

To ensure data persistence, the program does not rely on a database. Instead, it stores the necessary information in a text (txt) or CSV file.

## Installation

1. Clone the repository:
git clone https://github.com/MiladRezaeian/company-agencies.git

2. Navigate to the project directory:
cd company-agencies

3. Compile and build the program using the preferred compiler.
4. Run the program.

## Usage

To use the program, execute the CLI command with the desired flags and parameters. For example:

- To list representatives in a specific region:
company-agencies --command=list --region=desired-region



- To retrieve detailed information about a representative:
company-agencies --command=get --region=desired-region --id=representative-id



- To create a new representative:
company-agencies --command=create --region=desired-region



- To edit the information of a representative:
company-agencies --command=edit --region=desired-region


- To obtain the status of representatives in a region:
company-agencies --command=status --region=desired-region



## Data Storage

The program does not utilize a database for data storage. Instead, it stores the necessary information in a text (txt) or CSV file. The program ensures that the data persists even after exiting and restarting the program.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.

## License

This project is licensed under the [MIT License](LICENSE).
