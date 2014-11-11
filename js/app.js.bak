(function(){
//Model

  var Task = Backbone.Model.extend({
    defaults: {
      title: 'do something',
      completed: false
    }
  });

  var task = new Task();

// View
  var TaskView = Backbone.View.extend({
    tagName: 'li',
    events: {
      "click .command": 'sayHello'
    },
    sayHello: function(){
      alert('hello');
    },
    template: _.template($('#task-template').html()),
    //<<%- title %>
    render: function(){
      var template = this.template( this.model.toJSON() );
      this.$el.html(template);
      return this;
    }
  });

  // var taskView = new TaskView({model: task});
  // console.log(taskView.render().el);
  // $('body').append(taskView.render().el);

// Collection

  var Tasks = Backbone.Collection.extend({
    model: Task
  });

  var TasksView = Backbone.View.extend({
    tagName: 'ul',
    render: function(){
      this.collection.each(function(task){
        var taskView = new Taskview({model: task});
        this.
      });
    }
  });
  var tasks = new Tasks([
      {
        title: 'task',
        complete: true
      },
      {
        title: 'task2'
      },
      {
        title: 'task3'
      }
  ]);
  console.log(tasks.toJSON());

})();