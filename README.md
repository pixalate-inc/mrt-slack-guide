MRT Slack Bot Plugin
===

The MRT Slack Bot Plugin allows you to access MRT data directly within slack, as well as keep track of your top follows.

## Installation
You can install the MRT Slack Bot to your workspace by click the below button and following the prompts:

<a href="https://slack.com/oauth/v2/authorize?client_id=4596232674.1734105936803&scope=commands,links:read,links:write&user_scope=links:read,links:write"><img alt="Add to Slack" height="40" width="139" src="https://platform.slack-edge.com/img/add_to_slack.png" srcSet="https://platform.slack-edge.com/img/add_to_slack.png 1x, https://platform.slack-edge.com/img/add_to_slack@2x.png 2x" /></a>

## Account Linking
You can either link your account using the `/mrt account` command and clicking "Login", or by click the "Log In" button on the Home page. From there, the linking process will continue in your browser. Follow the on-screen prompts to link your MRT account to Slack.

## Commands

### Help

The help command displays all available commands along with a condensed description of their functionality.

#### Usage
```
/mrt help
```

#### Sample Output
```
/mrt help                           displays this help dialog
/mrt app <name|bundle_id|app_id>    retrieve details about an app  
/mrt ctv <id>                       retrieve details about a ctv app  
/mrt domain <domain>                retrieve details about a domain  
/mrt account                        manage the connection with your MRT account
```

### App Search

The App Search command allows you to retrieve general information about an App Store or Google Play app from within Slack. It also includes a link to view the app within the MRT, as well as the ability to follow the app from within Slack.

The details provided in the output are a brief overview of key metrics associated with the app. These cannot be customized at this time.

You may pass either the app name, the bundle id, or the app id to retrieve the associated app. Partial titles may be used, but for best results provide explicit app names or complete app/bundle ids.

#### Usage
```
/mrt app <name|bundle_id|app_id>
```

#### Sample Output

![MRT App Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_app_preview.png?raw=true)

### CTV Search

The CTV Search command allows you to retrieve general information about a Roku or Fire TV app from within Slack. It also includes a link to view the app within the MRT, as well as the ability to follow the app from within Slack.

The details provided in the output are a brief overview of key metrics associated with the app. These cannot be customized at this time.

CTV search only supports passing explicit app ids to retrieve the associated app at this time.

#### Usage
```
/mrt ctv <id>
```

#### Sample Output
![MRT CTV Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_ctv_preview.png?raw=true)

### Website Search

The Website Search command allows you to retrieve general information about a website from within Slack. It also includes a link to view the domain within the MRT, as well as the ability to follow the domain from within Slack.

The details provided in the output are a brief overview of key metrics associated with the domain. These cannot be customized at this time.

#### Usage
```
/mrt domain <domain_name>
/mrt website <domain_name>
```

#### Sample Output
![MRT Domain Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_domain_preview.png?raw=true)

### Account

The Account command allows you to manage your connection between the MRT and Slack.

#### Usage
```
/mrt account
/mrt login
/mrt logout
```

#### Sample Output
![MRT Account Logged Out Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_account_logged_out.png?raw=true)
![MRT Account Logged In Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_account_logged_in.png?raw=true)

## Home
Your MRT Slack home page can show you a summary of your top follows, as well as convenient links to view them in the MRT console when you've connected your account.

Home will always show your top three follows from each category. Currently, this is not configurable.

#### Configuring your Home
By pressing the Configure button at the top of the page, you are able to reorder or hide the sections you see in Home.

![MRT Configure Button Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_configure_btn.png?raw=true)

![MRT Configure Window Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_configure_window.png?raw=true)

You can reorder or hide each section by pressing the `...` menu to the right of each row. From there, you can see options to move or hide the section.

![MRT Reorder Dropdown Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_reorder_dropdown.png?raw=true)

If you've hidden a section, you can restore it via the "Add a section..." dropdown.

![MRT Restore Section Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_restore_section.png?raw=true)

Additionally, you can reset the layout to default using the Reset Layout button.

![MRT Reset Layout Preview](https://github.com/pixalate-inc/mrt-slack-guide/blob/master/Images/mrt_reset_layout.png?raw=true)

Once you're satisfied, you can save your new layout by pressing the Save button. You can also discard any changes you've made with the Cancel button, or by clicking the X button in the upper right.
