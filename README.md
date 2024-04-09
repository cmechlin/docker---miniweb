# Docker Web Server

This Docker container is a super lightweight web server based on BusyBox and HTTPd. It is designed specifically for serving static web files.

## Usage

1. Build the Docker image:

   ```bash
   docker build -t web-server .
   ```

2. Run the Docker container:

   ```bash
   docker run -d -p 80:80 -v /path/to/web/files:/var/www/html web-server
   ```

   Replace `/path/to/web/files` with the path to your static web files.

3. Access the web server:

   Open your web browser and navigate to `http://localhost`.

## Customization

You can customize the web server by modifying the configuration files located in the `conf` directory.

## License

This project is licensed under the [MIT License](LICENSE).
