<b>The base concept behind the 'ClosedEmailAddressProtocol' </b><br/>
<br/>
The concept is a very simple one. <br/>
<table>
 <tr>
  <td bgcolor="white" wrap=nowrap>Open RFC822 Email address</td><td bgcolor="white" wrap=nowrap>someone@somedomain.com </td>
 </tr>
 <tr>
 <td  bgcolor="white" wrap=nowrap>Closed RFC822 Email Address</td><td bgcolor="white" wrap=nowrap><i>hash_access_code</i>&#35;someone@somedomain.com</td>
 </tr>
</table>
<br/>
<br>
The <i>hash_access_code</i> would be a symetric hash using the current encryption technology.<br/>
<br/>
Existing *nix based ESMTP daemons would either be directly patched to understand this extension or have configuration rules added.<br/>
<br/>
For Winx systems either a custom ESMPT server would be created, patched or like sendmail its configuration could be extended to understand the access_code.<br/>
<br/>
This simple additon effectively closes down an email making unsolicited emails Spam unable to effect delivery.<br/>
With appropriate business process a 'rolling code of the day' could be utilized so that unsolitcited emails could not gain a lock on an open email.<br/>
<br/>
The hashed access code could be either generated by a separate desktop utility, script, Phone/Tablet based app or browser/email client extension<br/>
<br/>
This idea was originally developed back in 2003/2004, but the extra step of generating access code at the time proved to be a step to far for most end users to grasp.<br/>
Fast forward 18+ years, the end-user landscape has now changed dramatically with a much younger and technically aware population in place.<br/>
With updated and open source components with multiple contributors, the goal of this project would be to revamp the initial concept and bring it back into both technical
reality and practical use.<br/>.
<br/>
Along with this basic concept can be found the initial provisional patent document (with IP Attorney information redacted for confidentiallity). <br/>
Initial program code (VB6 and Perl 5). for both a Windows based ESMTP server (Typhoon), and hosted solution originally called 'CalicoMail' that utilized sendmail and Perl 5.<br/>

<br/>
The concept in a nutshell:<br/>
<br/>
Effectively the symetric_hash acts as a 'lid' on your email box. Providing protection against Spam and Phishing emails.<br/>
For an organization, the symetric_hash could be a rolling value like a code of the day.<br/>
<br/>
<table>
<tr><td wrap=nowrap valign=top>Traditonal 'Open Email Address'</td><td wrap=nowrap valign=top>CEAP 'Closed Email Address'</td></tr>
<tr><td wrap=nowrap valign=bottom>myuser@mydomain.com</td><td wrap=nowrap valign=top>s<br/>
                                                                        y<br/>
                                                                        m<br/>
                                                                        e<br/>
                                                                        t<br/>
                                                                        r<br/>
                                                                        i<br/>
                                                                        c<br/>
                                                                        _<br/>
                                                                        h<br/>
                                                                        a<br/>
                                                                        s<br/>
                                                                        h<br/>#myuser@mydomain.com</td></tr>
</table>
