This simple web-server let user experience such data-structures as stack and linked list;

  #Stack
    <bold>GET</bold>: `\stack\top`
    Lets user peek the top element of stack;
    <bold>GET</bold>: `\stack\size`
    Lets user check the size of stack;
    <bold>GET</bold>: `\stack\pop`
    Removes the top element of stack and returns to the user;
    <bold>POST</bold>: `\stack\`, awaits a string or number as a parameter;
    Push an item to the stack.

  #Linked List
    <bold>POST</bold>: `\list\`, awaits a JSON in format of `{"successor": "1", "value": "5"}`;
    If there is a valid `successor`, it will put the `value` before it.
    If there is no `successor`, `value` will appear in the end of the list;
    <bold>GET</bold>: `\list\`
    Responds to user with a list;
    <bold>DELETE</bold>: `\list\:value`
    If there is `value`, it will be deleted;
