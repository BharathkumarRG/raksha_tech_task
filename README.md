# Dashboard Project

This project is a two-page dashboard with login functionalities, built using Nuxt.js and the Shardcn Vue package for the UI framework.

Demo Link: https://raksha-tech-task-bharathkumar.vercel.app

Sample Screenshots:
![image](https://github.com/user-attachments/assets/df2e5c93-356c-4585-b91a-71ed01670614)
![image](https://github.com/user-attachments/assets/4c49801d-95a6-4184-92f7-3d79dbd428c3)
![image](https://github.com/user-attachments/assets/bbe2d1cd-1c16-4447-b836-36e8c5a8173c)


## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Running the Project](#running-the-project)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Features

- User authentication (login)
- Responsive dashboard interface
- Two main pages with different functionalities
- Built using Nuxt.js for server-side rendering
- Styled with Shardcn Vue for a modern UI

## Installation

To get started, clone the repository and install the dependencies using `bun`.

```bash
git clone https://github.com/yourusername/dashboard-project.git
cd dashboard-project
bun install
```

## Running the Project

To run the project locally, use the following command:

```bash
bun dev
```

This will start the development server, and you can view the dashboard at `http://localhost:3000`.

## Building for Production

To build the project for production, use:

```bash
bun build
```

This will create a production-ready build of the project in the `dist` directory.

## Project Structure

```
.
├── assets          # Assets such as images, fonts, etc.
├── components      # Vue components
├── layouts         # Layouts for the application
├── middleware      # Middleware for handling authentication
├── pages           # Application pages
├── plugins         # Plugins to extend functionality
├── static          # Static files
├── store           # Vuex store for state management
├── nuxt.config.js  # Nuxt.js configuration file
└── package.json    # Project metadata and dependencies
```

## Technologies Used

- [Nuxt.js](https://nuxtjs.org/) - A framework for creating Vue.js applications
- [Shardcn Vue](https://shardcn.com/) - A UI framework for Vue.js
- [Bun](https://bun.sh/) - A fast, all-in-one JavaScript runtime

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure that your code adheres to the project's coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

---
