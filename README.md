# notion
empty(prop("End")) ? "free" : if(formatDate(end(prop("End")), "YYYY,MM,DD") == formatDate(now(), "YYYY,MM,DD"), "D-day", if(end(prop("End")) < now(), concat("D+", format(dateBetween(end(prop("End")), now(), "days") * -1)), concat("D-", format(dateBetween(end(prop("End")), now(), "days") + 1))))
