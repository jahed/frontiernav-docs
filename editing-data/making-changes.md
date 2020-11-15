---
description: How to contribute data to FrontierNav.
---

# Making Changes

{% hint style="warning" %}
The process around Changes, Change Requests and Conflicts are being worked on. If you have any feedback to improve the process, get in touch.
{% endhint %}

## Communication

If you're making any changes, you should contact the community to share your ideas. Otherwise, it may result in duplicated effort or invalid data. That doesn't mean you have to have a conversation, more just an announcement so people are aware and can flag any potential problems.

## Change Model

FrontierNav's Change Model is append-only, meaning when you make a change, the next change requires the previous change. This ensures that changes are valid as a whole.

You can see the changes you've made by opening the Changes Sidebar from the Navigation Bar. Your changes are only local to you, no one else can see them unless if you create a change request and it's accepted \(read below\).

## Saving Changes

It's a good idea to regularly save your changes to keep a backup. If anything goes wrong down the line, you can always send the saved ZIP to an Admin to recover your changes.

## Autosaved Sessions

Your open changes are automatically saved every 10 seconds for the current session, up to a maximum of 5 autosaved sessions. After which the oldest session is removed.

This is a safety net in case your web browser crashes or you accidentally close your tab. Don't rely on it too much as web browsers have limited storage. After doing substantial work always Export manually to have a safe copy on your device.

## Opening Changes

You can open your saved ZIP to **continue where you left off**. That means any new data since your save won't be available.

To apply your changes on top of the latest data, you can extract and open the **changes.json** from your ZIP save.

## Resolving Conflicts

When opening **changes.json** on its own, your changes are re-applied over the latest published data. This means your changes might conflict if there's any new data. For example, you might have created a "Small Potion" entity, but then someone else also made one and published it first.

Whenever your changes conflict, you'll need to discard them to continue. To avoid losing your changes, you'll be given the option to **Save** them, after which you can send them to an Admin to fix.

## Rewinding Changes

If you make a mistake and want to go back to a previous state, you can open up the Changes Sidebar, **LeftClick** on the change you want to go back to and **LeftClick** "Rewind". This will reset the data and re-apply all of your changes up to that point and discard the rest.

{% hint style="info" %}
In the future, this interface will be improved to be more obvious.
{% endhint %}

## Change Requests

In order to publish your changes for others to see, you need to create a Change Request. Once you have done so, notify an Admin so that we're aware of it. Admins might be busy and may not respond immediately so give it up to a day before contacting again.

Your request will go through multiple stages:

* Pending: Your request is awaiting approval by an Admin.
* Rejected: An Admin rejected your request. The request will be updated with a reason.
* Accepted: Your request has been accepted.

You can discard your changes once you've made a Change Request. If you need to recover your changes, you can do so by clicking **Open** on the Change Request. This will apply your changes on top of the latest data, similar to opening a **changes.json**.

{% hint style="info" %}
In the future, most users may be given permission to accept Change Requests to speed up the process.
{% endhint %}

