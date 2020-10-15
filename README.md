# speeddating_AI2

## General

Author: Yap Jheng Khin

Note that this is the continuation from Part 1, which was done in <a href="https://github.com/polarBearYap/speeddating_AI">here</a>.
I have also discover many mistakes from part I, and part II will serve as an <b>improvement</b> or postmortem.

List of mistakes that I have made in part I are:

* Preprocess on whole dataset, which cause train-test contamination.</li>
* Perform cross validation instead of nested cross validation.</li>

My learning expection in Part II are:

* Discover various ways to detect correlated features.
* Perform feature selection to reduce model complexity.
* Apply nested cross validation on areas like hyperarameter tuning.
* Discover XAI techniques that can be used in explaining black box models.

## Metadata

* This data was gathered from participants in experimental speed dating events from 2002-2004.

* During the events, the attendees would have a four-minute "first date" with every other participant of the opposite sex. At the end of their four minutes, participants were asked if they would like to see their date again. They were also asked to rate their date on six attributes: Attractiveness, Sincerity, Intelligence, Fun, Ambition, and Shared Interests.

* The dataset also includes questionnaire data gathered from participants at different points in the process. These fields include: demographics, dating habits, self-perception across key attributes, beliefs on what others find valuable in a mate, and lifestyle information.

## Attribute Information

There are totally 56 preprocessed features which have undergone the data preprocessing in the dataset such as 'd_ funny' which show the particular attributes in discrete form. The dataset also 'has_ null' which represents whether the particular sample consisting null values. Several features with 'expected_' means the expectations of the users towards partners.

<table style="width: 35%; float: left; display: inline-block">
  <tbody><tr>
    <th>Features' Type</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>age-related features</td>
    <td>age, age_o, d_age</td>
  </tr>
  <tr>
    <td>unknown feature</td>
    <td>wave</td>
  </tr>
   <tr>
    <td>field</td>
    <td>field_sociology, field_money</td>
  </tr>
  <tr>
    <td>interest-related features</td>
    <td>shopping, music</td>
  </tr>
  <tr>
    <td>partner-related features</td>
    <td>intelligence_partner, funny_partner</td>
  </tr>
  <tr>
    <td>race-related features</td>
    <td>race, importance_same_race</td>
  </tr>
  <tr>
    <td>features about partner's preference</td>
    <td>pref_o_intelligence, pref_o_ambitious</td>
  </tr>
  <tr>
    <td>features about partner's rating on self</td>
    <td>intelligence_o, funny_o</td>
  </tr>
  <tr>
    <td>features about self's preference</td>
    <td>ambition_important, funny_important</td>
  </tr>
  <tr>
    <td>features about self's rating on herself/himself</td>
    <td>funny, intelligence</td>
  </tr>
</tbody></table>

## Source of the Dataset
* Published by: [Joaquin Vanschoren](https://www.openml.org/u/2) @ 2016 on https://www.openml.org/d/40536
   
* Available at:
  - [csv, arff](https://www.openml.org/data/get_csv/13153954/speeddating.arff)
  - [json](https://www.openml.org/d/40536/json)
  - [xml](https://www.openml.org/api/v1/data/40536)
  - [rdf](https://www.openml.org/d/40536/rdf)
  
* This dataset is also available at [kaggle](https://www.kaggle.com/polarbearyap/speed-dating)

## Relevant Paper
   * Raymond Fisman; Sheena S. Iyengar; Emir Kamenica; Itamar Simonson. Gender Differences in Mate Selection: Evidence From a Speed Dating Experiment.
   The Quarterly Journal of Economics, Volume 121, Issue 2, 1 May 2006, Pages 673–697, https://doi.org/10.1162/qjec.2006.121.2.673
