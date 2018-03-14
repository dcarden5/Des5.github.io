![photo](/images/capstone/The One In 100years Storm.png)

Predicting the 'One in One Hundred Year Storm' is nearly impossible.  Recently it seems that these 'One in One Hundred Year Storms' have come more frequently or at least not every one hundred years.  Hurricane Katrina occurred in 2005, but before that came Hurricane Camille in 1969, Labor Day Hurricane in 1935 in order of most devastating. Not so much 1 in 100, but each caused crippling losses.  

Can we come up with a reasonable approximation with data freely available on the web?  I believe that I could.  My storm analogy is applied to the management liability insurance space in this post.  My problem statement is: To provide an approximation or predictive model that estimates whether a Securities Class Action lawsuit settles or dismisses, using both non-parametric and parametric algorithms.  The ability to predict whether an SCA settles or dismisses has direct business implications for an insurance claims department.  As an insurance company receives claims, their claim department has to allocate reserve amounts normally associated with attorney fees and settlement costs.  Knowing whether an SCA settles or dismisses will assist an insurance company to reserve appropriately and not over or under leverage reserving cash.

What is management liability insurance, you ask? Management liability insurance products protect the publicly traded company from insolvency, its board of directors and C-level suites.  Share holders of these publicly traded companies can launch securities class action (SCAs) lawsuit against the corporation under a variety of legal theories.  These legal theories largely fall under a breach of fiduciary duty which "prohibits any act or omission resulting in fraud or deceit in connection with the purchase or sale of any security."

So far we have identified, at a business level, some of the moving parts to the "One in One Hundred Year Storm."  But what about the data?  Where can we attain this data on the web?  Yes, the Stanford Law School / Cornerstone Research site (http://securities.stanford.edu/) provides most of what we need to capture in order to be able to perform meaningful predictions related to the SCAs. The site contains about 4,500 SCAs from years 1996 up to the current month.  For purposes of this analysis, we have captured from 1996 to mid-2017.  The data points are as follows.

Company-public corporations that have been subjected to an SCA.  
Status-category that states whether the SCA is ongoing, settled or dismissed.  
Company market-refers to the Stock Exchange in which the company trades. 
Settlement Date-if the status is settled, then this date depicts when the company came to an agreement to pay shareholders for breach of 	fiduciary duty.  If the status is dismissed, then the date depicts when the judge has dismissed the case from proceeding any further 	based on the facts of the case.
Company sector-a broad (12) industry sector of publicly traded company.
Industry sector-a more detailed categorization of industry in which the corporation operates.
Headquarter-city of corporate headquarter
Ticker-stock symbol as used in respective trading exchange.
Court-details the state or federal venue in which the SCA was filed.
Docket-the case id number as assigned in court.
Judge-name of the judge administering to the SCA.
Date filed-refers to the date in which the SCA was filed in a federal venue.
Class period start-the date in which the fraud or deceit is alleged to have started.
Class period end-the date in which the fraud or deceit is alleged to have ended.
Case description-legal complaint with allegations raised in SCA lawsuit

![photo](/images/capstone/Stanford Law Clearinghouse Portal.png)
