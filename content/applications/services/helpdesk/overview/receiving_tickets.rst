=======================
Start receiving tickets
=======================

Helpdesk offers multiple channels where customers can reach out for assistance, such as email, live
chat, and through a website's submission form. The variety of these contact options provides
customers with multiple opportunities to receive support quickly, while also giving the support
team the ability to manage multi-channel support tickets from one central location.


Enable channel options to submit tickets
========================================

Go to :menuselection:`Helpdesk --> Configuration --> Teams` and choose an existing team, or click
:guilabel:`New` to :doc:`create a new team <getting_started>`.

On the team's settings page, scroll down to :guilabel:`Channels`. Select one or more channel to
enable and check the respective box(es).

   - :guilabel:`Email Alias`
   - :guilabel:`Website Form`
   - :guilabel:`Live Chat`


Email Alias
-----------

The :guilabel:`Email Alias` setting automatically creates tickets from messages sent to that team's
specified email alias.

To alter a helpdesk team's email alias, navigate to the :guilabel:`Teams` settings page. Find
:guilabel:`Email Alias` under the :guilabel:`Channels` heading.

When a new Helpdesk team is created, an :guilabel:`Email Alias` is created as well. This alias can
be changed in the :guilabel:`Alias` field.

.. note::
   If the database does not have a custom domain already configured, click
   :guilabel:`Configure a custom domain` to be redirected to the :guilabel:`Settings` page. From
   there, enable :guilabel:`Custom Email Servers`.

.. image:: receiving_tickets/receivingtickets-emailalias.png
   :align: center
   :alt: View of the settings page of a helpdesk team emphasizing the email alias feature
         in Odoo Helpdesk

When an email is received, the subject line from becomes the title of a new
helpdesk ticket. The body of the email is added to the ticket in the :guilabel:`Description` and
:guilabel:`Chatter`.

.. important::

   The configuration steps outlined above are for **Odoo Online** and **Odoo.sh** databases. For
   **On-premise** databases, additional configuration for custom email servers and email aliases
   may be required.


Website Form
------------

Enabling the :guilabel:`Website Form` setting adds a new page to the website with a customizable
form. A new ticket is created once the required fields on the form are completed.

To activate the website form, navigate to a team's settings page. Find the :guilabel:`Website Form`
feature under the :guilabel:`Channels` section and check the box.

After the feature is activated, click the :guilabel:`Go to Website` smart button on the team page.
The settings page may need to be refreshed before the :guilabel:`Go to Website` smartbutton appears.

.. image:: receiving_tickets/receivingtickets-gotowebsite.png
   :align: center
   :alt: View of the settings page of a helpdesk team emphasizing the Go to Website button in
         Odoo Helpdesk


A default website form  will be created for users to submit tickets. To customize the form, click
the :guilabel:`Edit` button in the upper right corner of the page. Then click on one of the fields
in the form.

Add, remove or update fields as necessary to alter the information submitted by customers. Fields
can be made *required* by *marking* them with preselected text.

.. image:: receiving_tickets/receivingtickets-webform.png
   :align: center
   :alt: View of the unpublished website form to submit a ticket for Odoo Helpdesk


Once the form has been updated, :guilabel:`Save` the changes, then publish the form by clicking on
the :guilabel:`Unpublished` button.


Live Chat
---------

The :guilabel:`Live Chat` application allows website visitors to connect directly with a support
agent or chatbot. During these conversations, Helpdesk tickets can be instantly created using a
Now, operators can create tickets by using the
:doc:`command </applications/websites/livechat/overview/responses>` `/helpdesk`.

To enable :guilabel:`Live Chat`, navigate to the :guilabel:`Teams` settings page. Click the check
box next to :guilabel:`Live Chat` under the :guilabel:`Channels` heading.

.. note::
   If this is the first time :guilabel:`Live Chat` has been enabled on the database, the page may
   need to be saved manually and refreshed before any further steps can be taken.

Click :guilabel:`View Channels`. Once on the :guilabel:`Website Live Chat Channels` page, select
the kanban card for the channel that was created for the helpdesk team. The name will match the
team name, though it can be changed.

.. example::
   For the Helpdesk team named `Customer Care`, a :guilabel:`Live Chat` channel was created with
   the same name.

   .. image:: receiving_tickets/receivingtickets-livechat-join-channel.png
      :align: center
      :alt: View of the kanban cards for the available Live Chat channels

On the Channel form, navigate through the tabs to complete the setup.

Add operators
~~~~~~~~~~~~~

:guilabel:`Operators` are the users who will act as agents and respond to live chat requests from
customers. The user who originally created the channel will be added by default.
To add additional users, navigate to the :guilabel:`Operators` tab, and click :guilabel:`Add`.
Click the check box next to the users to be added, and click :guilabel:`Select`.

.. tip::
   Users can add themselves as an operator by clicking the :guilabel:`Join` button on a
   :guilabel:`Live Chat` channel.

Modify channel options
~~~~~~~~~~~~~~~~~~~~~~

The :guilabel:`Options` tab contains the visual and text settings for the live chat button and
window.
Change the text in the :guilabel:`Text of the Button` field to update the greeting displayed in
text bubble when the live chat button appears on the website.

Edit the :guilabel:`Welcome Message` to change the message a visitor sees when they open the chat
window. This message will appear as though it is sent by a live chat operator, and should be an
invitation to continue the conversation.

Edit the :guilabel:`Chat Input Placeholder` to change the text that appears in the box where
visitors will type their replies.
Change the color of the live chat button and window header by clicking the a circle to open the
color selection window. Click the button to the right to reset to the default color selection.

.. tip::
   Color selection, for the button or header, can be made manually, or through RGB, HSL or HEX code
   selection. To change the color selection options click on the arrow buttons.

      .. image:: receiving_tickets/receivingtickets-change-color.png
         :align: center
         :alt: Focus on the color changing options for livechat button and window

.. example::
   The screenshots below show where the inputs for the :guilabel:`Options` tab are displayed on the
   live chat button and live chat window.


   .. image:: receiving_tickets/receivingtickets-livechat-optionstab.png
      :align: center
      :alt: View of the kanban cards for the available Live Chat channels

   .. image:: receiving_tickets/receivingtickets-livechat-textinput-examples.png
      :align: center
      :alt: View of the kanban cards for the available Live Chat channels


Create channel rules
~~~~~~~~~~~~~~~~~~~~

The :guilabel:`Channel Rules` is where rules and actions for the channel are defined.
Click :guilabel:`Add a line` to create a new rule.

Choose how the :guilabel:`Live Chat Button` will be displayed on the website.

If a :guilabel:`Chatbot` will be included on this channel, select it from the dropdown. If the
chatbot will only be active when no operators are available, check the box labeled
:guilabel:`Enabled only if no operator`.

Add the url for the pages this channel will be applied to in the :guilabel:`URL Regex` field.
If this channel will only be available to users in specific countries, add them to the
:guilabel:`Country` field. If this field is left blank, the channel will be available to
all site visitors.

.. image:: receiving_tickets/receivingtickets-channel-rules.png
   :align: center
   :alt: View of the kanban cards for the available Live Chat channels

Use the live chat widget
~~~~~~~~~~~~~~~~~~~~~~~~

The live chat :guilabel:`Widget` can be applied to websites created through Odoo by navigating to
the :menuselection:`Website application --> Configuration --> Settings`. Scroll to
:guilabel:`Live Chat` and select the channel to add to the site. Click :guilabel:`Save`.

To add the widget to a website created on a third-party platform, click :guilabel:`copy` and paste
the code into the <head> tag on the site.


Creating a ticket from a conversation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Once live chat is enabled, operators will be able to communicate with site visitors in real time.
During the conversation, an operator can use the shortcut
:doc:`command </applications/websites/livechat/overview/responses>` `/helpdesk` to create a ticket
without leaving the chat window. The transcript from the conversation will be added to the new
ticket.


Prioritizing tickets
====================

All tickets include a :guilabel:`Priority` field. The highest priority tickets will appear at the
top of the kanban and list views.

.. image:: receiving_tickets/receivingtickets-priority.png
   :align: center
   :alt: View of a team's kanban view and the prioritized tasks in Odoo Helpdesk

The priority levels are represented by stars:

   - 0 stars = *Low Priority*
   - 1 star = *Medium Priority*
   - 2 stars = *High Priority*
   - 3 stars = *Urgent*

Tickets will be set to low priority (0 stars) by default. To change the priority level, select the
appropriate number of stars on the kanban card, or on the ticket.

.. warning::
   As priority levels can be used as criteria for assigning :doc:`SLAs <sla>`, changing the
   priority level of a ticket can alter the SLA deadline.

.. seealso::
   - :doc:`sla`
   - :doc:`../advanced/close_tickets`
   - :doc:`/applications/general/email_communication/email_servers`
   - :doc:`/applications/websites/livechat/overview/get_started`
