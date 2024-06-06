# QUIL Node Backups

This is a basic backup script that creates a new folder in the `$HOME` directory with the current date as the name, then backs up specific configuration files and directories.

## Files and Directories Backed Up

- `~/ceremonyclient/node/.config/config.yml`
- `~/ceremonyclient/node/.config/keys.yml`
- `~/ceremonyclient/node/.config/store`

## Usage

1. **Clone the Repository**

    ```sh
    wget https://raw.githubusercontent.com/TidalWavesNode/QUIL_backups/main/backing_up.sh
    ```

2. **Make the Script Executable**

    ```sh
    chmod +x backing_up.sh
    ```

3. **Run the Script Manually**

    You can run the script manually to test it:

    ```sh
    ./backing_up.sh
    ```

## Scheduling the Script with Cron

To automate the script to run daily, you can set up a cron job:

1. **Open the Crontab Editor**

    ```sh
    crontab -e
    ```

2. **Add the Cron Job**

    Add the following line to schedule the script to run daily at 2 AM:

    ```sh
    0 2 * * * /bin/bash /path/to/your/backing_up.sh
    ```

    Replace `/path/to/your/backing_up.sh` with the actual path to the `backing_up.sh` file.

3. **Save and Exit**

    Save the file and exit the editor. This will set up the cron job to run the script daily at 2 AM.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or enhancements.

## Author

Created by [TidalWavesNode](https://github.com/tidalwavesnode).