# Tassker

## Description
To-do list manager.

## Task
The requirements to the application are described [here](https://drive.google.com/file/d/18I1PxOxZn2lwm__YeOtMNoWeiXygKwwN/view).

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

## Application stack
Besides **Firebase** platform and **React** library (create-react-app was used as a boilerplate) the following tools were applied for developing the application:
- **React Router** for client-side routing;
- **Bootstrap** components and icons formed the basis of application interface;
- **Formik** library was utilized to handle forms data;
- **classnames** package was used for conditional addition of React components classNames;
- **moment.js** for dates processing.