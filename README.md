# Uncommon HTML Bug: Event Listener on Dynamically Created Element

This repository demonstrates an uncommon bug in HTML related to adding event listeners to dynamically created elements.  The incorrect approach involves adding an event listener to an element before it exists in the DOM. This can lead to the event listener not functioning as expected. The solution showcases the correct way to attach the event listener.  

## Bug Description
The primary issue is that attempting to attach an event listener to an element that does not yet exist at the time the script executes will result in the event listener being registered to null. Therefore, the click event won't fire. This is different from a typical 'element not found' error, and is often tricky to debug.