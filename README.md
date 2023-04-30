#Instructions to run this code
1. Copy the code and paste it into a JavaScript file (e.g., detectCycle.js);
2. Save the file;
3. Create a new HTML file (e.g., index.html) in the same directory as the JavaScript file;
4. Add a <script> tag to the HTML file and set the "src" attribute to the name of the JavaScript file: <script src="detectCycle.js"></script>;
5. Create a ListNode instance and a cycle by connecting a node to itself, for example:
const head = new ListNode(1);
const node2 = new ListNode(2);
head.next = node2;
const node3 = new ListNode(3);
node2.next = node3;
const node4 = new ListNode(4);
node3.next = node4;
node4.next = node2; // create a cycle;
6. Call the detectCycle function with the head node as an argument:
const cycleNode = detectCycle(head);
7. The function will return the node where the cycle begins or null if there is no cycle. You can then print or use the cycleNode as desired:
console.log(cycleNode); // should output the node with val = 2.



