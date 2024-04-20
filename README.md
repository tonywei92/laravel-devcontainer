# Laravel Development Container Example

Welcome to the Laravel Development Container Example repository! This repository is designed to provide a quick and efficient way to set up your Laravel development environment using Docker and Visual Studio Code DevContainers. The provided configuration streamlines the setup process, ensuring that you have a consistent and isolated development environment that mirrors Laravel's server requirements.

## Introduction

Developing with Laravel requires a specific set of PHP extensions and configurations to ensure compatibility and performance. To simplify the development setup, we've provided a DevContainer configuration that encapsulates all the necessary extensions and settings, following the [official Laravel documentation](https://laravel.com/docs/11.x/deployment#server-requirements). This setup allows you to focus more on development and less on configuring your environment.

## How to Use the DevContainer Configuration

To get started with the provided DevContainer configuration, follow these steps:

1. **Copy the `.devcontainer` folder** into the root of your Laravel project. This folder contains all the necessary configuration files for your development environment.

2. **Reopen the project in DevContainer** by using Visual Studio Code:
   - On **Mac**, press `CMD+SHIFT+P`.
   - On **Windows and Linux**, press `CTRL+SHIFT+P`.
   - Then, choose `Dev Containers: Reopen in Container` from the command palette.

This process will create and start a Docker container based on the configuration specified in the `.devcontainer` folder. Once the container is running, your project will be reopened inside the container, providing an isolated development environment.

## Included PHP Extensions

The DevContainer configuration includes the following PHP extensions, essential for Laravel development:

- `libpq-dev`
- `libpng-dev`
- `libzip-dev`
- `imagemagick`
- `pdo`
- `pdo_pgsql`

These extensions are installed to meet Laravel's server requirements and ensure that your application runs smoothly both in development and production environments.

## Default PHP Version

The default PHP version in the DevContainer is **8.2**. If you need to use a different PHP version, you can easily adjust this by:

1. **Updating the Dockerfile** in the `.devcontainer` folder. Replace the PHP version with the one you require.
2. To find a complete list of available PHP versions, visit the [Microsoft official PHP devcontainers version list](https://mcr.microsoft.com/v2/devcontainers/php/tags/list).

After updating the PHP version, **rebuild the container** to apply the changes:

- On **Mac**, press `CMD+SHIFT+P`.
- On **Windows and Linux**, press `CTRL+SHIFT+P`.
- Choose `Dev Containers: Rebuild Without Cache and Reopen in Container` from the command palette.

This will rebuild the Docker container without cache, ensuring that the new PHP version is installed.

## Conclusion

With this Laravel Development Container setup, you can quickly start developing your Laravel applications without worrying about environment inconsistencies or configuration issues. The isolation provided by Docker and the ease of setup with VS Code's DevContainers offer a robust solution for Laravel development.
