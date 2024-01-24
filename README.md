# Leto Dashboard

## Setup and installation

```bash
npm install
```

## Run the Dashboard in Dev mode
- Turn off the authentication requirement to run the dashboard in a local dev environment
  - Locate the index.jsx file (src/components/templates/MainLayout)
  - Comment out the code in this file and add the following code

  ```
  import { Outlet } from "react-router-dom";
  function MainLayout() {
  // const { isAuth } = useAuth(); // No longer using the authentication check
  // Removed the check and redirect logic
  return <Outlet />;
  }
  export default MainLayout;
- Save the file and run in local host
  ```
  npm run dev 
