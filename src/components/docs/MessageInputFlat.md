```js
import { Chat } from '../Chat';
import { MessageTeam } from '../MessageTeam';
import { Channel } from '../Channel';
import { MessageInput } from '../MessageInput';
import { MessageInputFlat } from '../MessageInputFlat';

const data = require('./data');

<div className="str-chat" style={{ height: 'unset' }}>
  <Chat client={data.client} Message={MessageTeam}>
    <Channel channel={data.channel}>
      <MessageInput
        Input={MessageInputFlat}
        grow={true}
        focus={false}
        {...data.translationContext}
      />
    </Channel>
  </Chat>
</div>;
```
