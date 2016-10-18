# Graphs Documentation

## Import Highcharts library
* To import Highcharts in this project, make sure that the project imported jquery, then add the below code to ../app/View/Layouts/default.ctp:
    `<script src="<?php echo $this->webroot; ?>js/highcharts/highcharts.js"></script>`

## Matrix graphs
* In this graph, we use an ajax to get a feed from backend side first. Then use an array to contains the ranking number and others parameters. These others parameters in this array help us matching the ranking number and object easily.
* The below code is a peace of code to set data to the ranking number array:

    `ranking_number_collection.push({
       ranking_number: 0,
       feature_name: data[i]['Surveyfeature'].Feature_name,
       section_feature_score: data[i]['SurveyfeaturesScore'].section_feature_score,
       feature_score: data[i]['SurveyfeaturesScore'].feature_score,
       section: data[i]['Surveyfeature'].Section,
       survey_feature_score_id: data[i]['SurveyfeaturesScore'].id
     });`

* After that, we use an array named `exist_section` to contains the name of sections which are in the shown object. There is a `section_number` parameter which is used as index of section to map the current dot with its section object:

    `if(exist_section.indexOf(survey_feature_item.Section) < 0) {
          exist_section.push(survey_feature_item.Section);
          plot_collection.push({
              name: survey_feature_item.Section,
              data: [{
                  ranking_number: ranking_number,
                  x: xAxis_plot,
                  y: yAxis_plot,
                  feature_name: feature_name,
                  feature_score: feature_score
              }]
          });
          x_collection.push(xAxis_plot);
      }else{
          var section_number = exist_section.indexOf(survey_feature_item.Section);

          if(plot_collection[section_number].name == survey_feature_item.Section) {
              plot_collection[section_number].data.push({
                  ranking_number: ranking_number,
                  x: xAxis_plot,
                  y: yAxis_plot,
                  feature_name: feature_name,
                  feature_score: feature_score
              });
              x_collection.push(xAxis_plot);
          }
      }`

# Reference Resources

* [CakePHP coding standards](http://book.cakephp.org/2.0/en/contributing/cakephp-coding-conventions.html)
