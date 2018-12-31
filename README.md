# React Joyride

[![](https://badge.fury.io/js/react-joyride.svg)](https://www.npmjs.com/package/react-joyride) [![](https://travis-ci.org/gilbarbara/react-joyride.svg)](https://travis-ci.org/gilbarbara/react-joyride) [![](https://api.codeclimate.com/v1/badges/43ecb5536910133429bd/maintainability)](https://codeclimate.com/github/gilbarbara/react-joyride/maintainability) [![](https://api.codeclimate.com/v1/badges/43ecb5536910133429bd/test_coverage)](https://codeclimate.com/github/gilbarbara/react-joyride/test_coverage)

[![Joyride example image](http://gilbarbara.github.io/react-joyride/media/example.png)](http://gilbarbara.github.io/react-joyride/)

#### Create awesome tours for your app!

Showcase your app to new users or explain functionality of new features.  

It uses [react-floater](https://github.com/gilbarbara/react-floater) for positioning and styling.  
And you can use your own components too!

**View the demo [here](https://2zpjporp4p.codesandbox.io/)**

**Read the [docs](https://gilbarbara.gitbook.io/react-joyride/)**

## Setup

```bash
npm i react-joyride
```

## Getting Started

```javascript
import Joyride from 'react-joyride';

export class App extends React.Component {
  state = {
    steps: [
      {
        target: '.my-first-step',
        content: 'This is my awesome feature!',
      },
      {
        target: '.my-other-step',
        content: 'This another awesome feature!',
      },
      ...
    ]
  };

  render () {
    const { steps } = this.state;

    return (
      <div className="app">
        <Joyride
          steps={steps}
          ...
        />
        ...
      </div>
    );
  }
}
```

## Documentation

[Props](docs/props.md)

[Step](docs/step.md)

[Styling](docs/styling.md)

[Customization](docs/customization.md)

[Callback](docs/callback.md)

[Constants](docs/constants.md)

[Accessibility](docs/accessibility.md)

[Migration from 1.x](docs/migration.md)

