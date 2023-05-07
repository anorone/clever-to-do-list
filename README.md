# Tassker

## Requirements
The requirements to the application are described [here](https://drive.google.com/file/d/18I1PxOxZn2lwm__YeOtMNoWeiXygKwwN/view).

## How to run the app
Live demo is available at [https://clever-to-do-list-1122b.web.app/](https://clever-to-do-list-1122b.web.app/).

## Database snapshot
Entities in the database are structured as follows:
```
{
  tasks: {
    [user.uid]: {
      [taskId]: {
        title: string,
        description: string,
        date: number,
        completed: boolean,
        id: string,
      },
      ... // other tasks
    }
  }
}
```

Live example:
![Screenshot from 2023-05-07 16-59-06](https://user-images.githubusercontent.com/89708037/236699165-52306138-5cf0-4901-bbde-cd5b83dc8ba1.png)

## Application stack
Besides **Firebase** platform and **React** library (create-react-app was used as a boilerplate) the following tools were applied for developing the application:
- **React Router** for client-side routing;
- **Bootstrap** components and icons formed the basis of application interface;
- **Formik** library was utilized to handle form data;
- **Classnames** package was used to conditionaly add React components classNames;
- **Moment.js** to process dates.
