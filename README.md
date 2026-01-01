# Klipper-Backup 💾 
Klipper backup script for manual or automated GitHub backups 

This backup is provided by [Klipper-Backup](https://github.com/Staubgeborener/klipper-backup).

The default [.env file](https://github.com/Staubgeborener/Klipper-Backup/blob/main/.env.example) is used with the proper configuration variables set at the top of the file. The .env file is located at `~/klipper-backup/.env`

The GitHub fine-grained access token lasts for one year. When you get the notification that it is about to expire, create a new token and update the `github_token` variable in your .env file (located at `~/klipper-backup/.env`).

# Z offset Calibration Instructions 📏

1. Home the printer.
2. From the console, type `PROBE_CALIBRATE` and press enter.
3. Use a piece of paper to gauge the distance between the nozzle and the bed.
4. Adjust the Z offset in the printer's settings until the paper has a slight drag when pulled out.
5. Type `SAVE_CONFIG` in the console to save the new Z offset.
6. Run the command `PROBE_ACCURACY` to verify the Z offset accuracy.
7. Fine-tune the Z offset as needed based on the first layer quality.