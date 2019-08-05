# react-router-debug-history
Import as <DebugHistory /> on the Component that are you trying to debug.

```javascript
import { useEffect } from 'react';
import { withRouter } from 'react-router-dom';

const DebugHistory = ({ history }) => {
  useEffect(() => {
    console.table(history);
  }, [history]);

  return null;
};

export default withRouter(DebugHistory);
```
